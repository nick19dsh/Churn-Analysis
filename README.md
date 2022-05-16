## Overview

Understanding why customers do—or don’t—purchase more goods or services is essential to success for any company. Gaining this insight begins with analyzing how many clients are taking their business elsewhere. Then, you can dig in to find commonalities among leavers, identify opportunities to improve and avoid losing additional customers.

Customer churn, or attrition, is the rate at which clients opt out of purchasing more of a company’s products or services. Customer churn analysis is a method of measuring this rate.

This project provides insights of churn_rate of customers from previous data and using this data, there is a classification analysis to evaluate performance of different ML algorithms.

### The Data

There is a single csv file that consist of different integer data like Senior_Citizen, Tenure, different floating type data like Monthly_Charges and Total_charges and different categorical data like Customer_ID, Churn, Contract, Payment Method, etc.

## Python libraries
-   Numpy
-   Pandas
-   Matplotlib
-   Seaborn
-   Scikit-Learn
-   XGBoost

## Project Introduction

The following different parts of this project consist of various steps from reading and analysing the data to the classication part.

### Part 1 - Imports and Read in the Data

In this part, data was imported using Pandas library to read different features of it.

### Part 2 - Quick Data Check

This part consist of checking the datatypes, non-null values and quick statistical summary of the numeric columns.

### Part 3 - Exploratory Data Analysis

In this part, there are some general feature exploration like:
+ Balance of the class label(Churn) with a Count Plot
+ Distribution of Total_charges between Churn categories with a Box Plot
+ Distribution of Total_charges per Contract type with a Box Plot
+ Correlation of features to the class label with a Bar Plot

### Part 4 - Churn Analysis

This part focuses on segmenting customers based on their tenure, creating cohorts and examining differences between customer cohort segments.

Cohort creation based on tenure means treating each unique tenure length 1 month, 2 month, 3 month...N months as its own cohort.

### Part 5 - Predictive Modeling

In this part, classification is done based on various supervised Machine Learning algorithms like:
+ Decision Tree
+ Random Forest
+ XGBoost

Evaluation of performance metrics is done by Classification Report and Confusion Matrix. Hyperparameter Tuning and Cross Validation are being used in XGBoost algorithm to balance the class and to get higher percentage of precision and recall.
