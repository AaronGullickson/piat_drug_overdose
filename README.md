# Putting It All Together Project on [Name of Research Project]

# Introduction

Throughout the the term, you will be working to build up an analysis of a specific research question, detailed below. You will complete several Putting It All Together assignments that ask you to analyze a dataset using the specific tools you have learned. For each assignment, you will report your results in a brief report. The ultimate goal of this set of assignments is a final complete research report on your specific research question. 

## Research Topic: 

Describe research topic

### Research questions

1. x related to y
2. contextual variable

## Technical Details

We will be using [R Markdown](https://rmarkdown.rstudio.com/) to write the actual reports as pdf documents. You should read in full the instructions for using R Markdown on the Canvas page. R Markdown will allow you to create professional quality reports with your tables and figures fully integrated. In this project, you will find a `full_report.Rmd` R Markdown file that you will use to produce your report. All assignments should be completed by knitting this report to PDF and submitting the PDF on Canvas. 

You can learn more about the dataset that you will be using by going to the README in the input directory, where you will also find the actual RData file itself. 

Please keep the following guidelines in mind for all project reports:

- Use clear, concise and accessible language throughout the report. Your target reader is not me, but rather a smart group of people who have little experience in interpreting statistics. Your job is to explain your results to them.
- Because you will be describing things that are already described from other sources, be sure to not accidentally plagiarize text. Describe everything in your own words.
- Do not refer to variables by their label in R (e.g. "indegree"). Do refer to variables in concrete meaningful ways (e.g. "number of friend nominations")
- Do not provide a narrative of your R script (e.g. "Then, I ran the tapply command to calculate mean differences between A and B "). Do present the results from your analysis in R in a way that someone who didn't know R from a hole in the ground would understand (e.g. "On average, members of A had XX more friend nominations than members of B").
- Do not use a casual tone. Do use a professional tone.

## Assignment 1: Introduction and Data

In this assignment, we will write an introduction for the report and begin the analysis of the data. You should use Introduction and Data sections of the `full_report.Rmd` file. You will also want to be sure to read the information about the variables and dataset provided in the README file in the `input` directory.

1. Write an introduction. This introduction should include a statement of the research question (in your own words) and a justification for why it is important to know the answer to this research question. Use your sociological imagination for the justification. The introduction should be 1-2 paragraphs.
2. Complete the data section of the research paper. The data section should include an overall description of the dataset (in your own words) being used to analyze the data as well as a description of the key variables used in the analysis. These key variables include the dependent (outcome) variable, the independent variable that is our primary explanatory variable as well as the variable we are considering as the contextual variable. All of these variables are identified in your research question above. You should include figures showing the distribution of each of these key variables as well as text that describes any key features of these distributions.

When you have completed the assignment, knit your report to PDF and upload it to the Canvas assignment page.

## Assignment 2: Measures of Association

In this assignment, we will continue the analysis of the data by beginning the Results section of the `full_report.Rmd`. We will now begin to explore the relationship between our key independent and dependent variable. You should do the following:

1. Examine ways to graphically show the relationship. Show figures in your report and describe what these figures tells you in words.
2. Estimate the bivariate measure of association between your variables and report the results in the text of the report.

When you have completed the assignment, knit your report to PDF and upload it to the Canvas assignment page.

## Assignment 3: Models and Full Report

You will now complete your report. In order to do that you should do the following.

1. Develop nested models that begin with your key variable and then add other variables in your dataset as controls to see how robust the result is to such controls. You should include at least two models (one with no controls and one with full controls), but you should also consider adding control variables in thematic blocks as this may help illuminate what variables are changing the relationship. You should also add a final model with an interaction term between your key independent variable and the contextual variable. Report your results in a regression model table using `knitreg` and describe the results in words.
2. Make corrections to all previous parts of the report based on instructor feedback and in order to maintain a consistent narrative.
3. Add a conclusion (1-2 paragraphs) that describes your ultimate findings as well as any weaknesses or concerns you have about the analysis and/or data.

When you have completed the assignment, knit your report to PDF and upload it to the Canvas assignment page.
