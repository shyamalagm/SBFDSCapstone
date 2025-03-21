---
title: "Capstone Project: San Francisco Police Department Incidents"
author: "Shyamala Gurumurthy"
date: "February 5, 2018"
output: 
  html_document: 
    highlight: tango
    keep_md: yes
    theme: cosmo
---



The city of San Francisco is not only known as a commercial and financial center of Northen California, but is also earning a growing reputation for having one of the highest crime rates in the country. The San Francisco Police Department (SFPD) is the city police department of San Francisco, that serves an estimated population of 1.2 million. The SFPD has been frequently met with criticism, due to the large number of cases that remain unsolved every year. For this reason, SFPD is determined to build trust, engage with the San Francisco community, and drive positive outcomes in public safety. In an effort to be as transparent as possible with information about the department and its operation, SFPD has shared [various data sets](https://data.sfgov.org/browse?Department-Metrics_Publishing-Department=Police%20Department). The [Police Department incidents](https://data.sfgov.org/Public-Safety/Police-Department-Incidents/tmnf-yvry) data is analyzed in this project.


### Dataset Description

This [dataset](https://data.sfgov.org/Public-Safety/Police-Department-Incidents/tmnf-yvry) derived from the SFPD Crime Incident Reporting System consists of a list of crime entries from 01/01/2003 up until 01/15/2018. It has around 2.18 million entries of incidents. There are 13 features that include the Category of crime, Date, Day of the week, Time, Location, Resolution etc. 

To aid in the inference of the effect of crime rate on the property prices, a [secondary dataset](https://www.zillow.com/research/data/) consisting of house prices was downloaded from [Zillow](https://www.zillow.com/)(see image below).

![Zillow dataset](zillow-data.jpg)


### Problem Statements

The possible goals for prediction for this dataset might include,

1. Predict the category of crime likely to occur in a given location, day-of-the-week and time-of-day.

2. Predict the number of crimes for a given category that will be resolved by given police district in each of the following years: 2015, 2016, 2017, and 2018 (note that there is no data for 2018 to validate results against!).

3. Infer if crime rate affect property prices in San Francisco. That is, to see if the areas that have low crime rates enjoy higher property values.

### Analysis and Model Building

The data wrangling method will involve identifying the variables that have an effect on the categories of crime. This will include creating new variables such as Year, Month, Date, etc. and deleting varibles that have no effect on the analysis such as Incident Number, Pdid, etc. I will also look for missing/outlier values(if any!) and replace/delete them appropriately. 

The Zillow dataset must be combined with the SFPD dataset to yield the property price corresponding to each crime location.

The exploratory data analysis will include time-series visualization of crime by category and location with the aim of answering goals mentioned above. Trends with seasonality and holidays will have to be specially considered for each year. The time of day is also expected to play an important role.

To simplify analysis, the dataset will be partitioned into training and testing portions. The training dataset will include incidents from year 2003-2014 and the testing dataset will include incidents from 2015-2018. The same split will be used for both the problem statements above. Several modeling approaches may be appropriate and will have to be explored. Clarity on the model building strategy will be obtained only as the analysis progresses.


### Deliverables

The final deliverables would include,

1. A comprehensive report in HTML (via RMarkdown) detailing the data transformations, exploratory data analysis and results of modeling that answer the queries above.

2. Complete R code used for all the analysis and modeling

Both items will be uploaded to Github.
