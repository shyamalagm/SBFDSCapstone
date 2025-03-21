---
title: "Capstone Project Proposals"
author: "Shyamala Gurumurthy"
date: "29 January, 2018"
output: 
  html_document: 
    keep_md: yes
    theme: yeti
---

## [Caravan Insurance](https://archive.ics.uci.edu/ml/datasets/Insurance+Company+Benchmark+(COIL+2000))


This dataset contains 9822 customer data records for an insurance company. Per possible customer, 86 attributes are given: 43 socio-demographic variables, and 43 variables about ownership of other insurance policies.

### Objective

The feature of interest is **whether or not a customer buys a Caravan insurance**. This task will be to predict whether someone will buy a caravan insurance policy.

### Exploratory data analysis

This will entail exploratory data analysis. Visualising the data should give some insight into certain particularities of this dataset. Of the 86 attributes, it is likely that many will not influence the response. EDA will help select features that would be useful in the context of the objective.
 
### Model building

Then data needs to be prepared for regression analysis. It will be important to select the right features, or to construct new features from existing ones.

## [SF Police Department Incidents](https://data.sfgov.org/Public-Safety/Police-Department-Incidents/tmnf-yvry)


This dataset contains incidents derived from SFPD Crime Incident Reporting system showing data from 1/1/2003 up until 1/8/2018.

### Objective

Possible goals for prediction might include,

1. Category of crime likely to occur in a given location, day-of-the-week and time-of-day.
2. Predict the number of crimes for a given category that will be resolved by given police district in each of the following years: 2015, 2016, 2017, and 2018 (note that there is no data for 2018 to validate results against!).

### Exploratory data analysis

EDA would include time-series visualization of crime by category and location with the aim of answering goals in the objective. Trends with seasonality and holidays will have to be specially considered for each year. The time of day is expected to play an important role.
 
### Model building

An appropriate subset of data will have to be determined and prepared of regression analysis. Important features need to be selected for predictions as per the objective.


## [OFLC PERM Disclosure Data](https://www.foreignlaborcert.doleta.gov/performancedata.cfm?CFID=160810&CFTOKEN=81367008)

PERM (Program Electronic Review Management) is an electronic processing system for filing labor certification applications for employment based green card.
Under the PERM system, labor certification applications are filed electronically and directly with the U.S. Department of Labor (DOL). This allows an employer to hire a foreign worker to work permanently in the United States.

### Objective

Possible prediction goals might include,

1. Visa decisions based on employee/employer/class of admission
2. Likelihood of given visa decision based employer/country of citizenship/city/sector

### Exploratory data analysis

EDA would include investigating features in relation to visa decisions. This would typically result in reducing the number of features that would be used in building the model. 

Based on trends and patterns observed, some features may warrant further study. Correlation tables between the features and visa decision response will also have to be explored. Based on these, new features may need to be created.
 
### Model building
After determining the features of interest, a regression model needs to be created with the aim of answering one or all the questions in the objective on a test dataset. This will include assessing the quality of the model.
