# Data Source Description

Data on the drug overdose death rate is derived from vital statistics data collected by the [Center for Disease Control and Prevention](https://www.cdc.gov/nchs/nvss/index.htm) (CDC). Data were extracted via the [CDC Wonder](https://wonder.cdc.gov/) system. The CDC only releases county level data publicly in counties large enough to maintain individual anonymity. In the case of death from overdose, this restriction means that not all counties are available for analysis. Particularly small counties in population size are excluded from the results, meaning that our sample of counties is biased toward larger, more metropolitan areas. You should keep this in mind in your analysis.

The remaining county level data is based on [American Community Survey](https://www.census.gov/programs-surveys/acs) (ACS) data for the years 2016-2020. The ACS is a 1-in-100 sample of the US population conducted annually by the US Census Bureau. At the county-level, the sample is small enough that estimates in smaller counties may suffer from sampling error. By pooling five years of data, we reduce the effect of this sampling error substantially. The data were extracted from the [Social Explorer](https://www.socialexplorer.com/explore-maps) system.

I have combined these data sources together into our full analytical dataset which is available in the `input` directory. To load this dataset in R, you just need to run the setup code chunk in the full_report.Rmd R Markdown document. The name of the dataset in R is `overdose`. The variables in this dataset are:

* **county**: The name of the county. This is not a variable you will use for the analysis, but helps to identify each county.
* **county_code**: The numeric id of each county. This is also not a variable you will use for the analysis, but is used to link records across multiple sources.
* **death_rate**: The number of deaths per 100,000 population from drug overdose in 2020. This is the key dependent variable. This death rate has been "age standardized" so that it is not the actual death rate but the expected death rate applied to a standard age distribution across counties. This removes differences across counties that may result from different death rates by age combined with some county populations being older or younger than others.
* **metro**: A categorical variable indicating whether the county was part of a metropolitan area or not. Counties that are part of metropolitan areas include both urban and suburban places and large and small cities (e.g. Multnomah county, Washington county, and Lane county in Oregon are metropolitan counties). This is the key contextual variable.
* **pop_density**: Number of people per square mile.
* **pct_nonwhite**: Percent of the population that is not white.
* **dropout_rate**: Percent of the population aged 16-19 that is not currently in school and does not have a high school diploma.
* **unemp_rate**: Percent of the labor force (those working or seeking work) that is currently unemployed.
* **pct_frgn_born**: The percent of the population that is foreign born.
* **poverty_rate**: The percent of the population who live in a household where the household income is below the federally defined poverty line. This is the key independent variable.
