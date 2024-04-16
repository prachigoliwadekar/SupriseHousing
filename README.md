# Surprise housing Case Study

## Table of Contents
* [Problem Statement](#problem-statement)
* [Objectives](#objectives)
* [Data Understanding](#data-understanding)
* [Data cleaning and manipulation](#data-cleaning-and-manipulation)
* [Data Analysis](#data-analysis)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Glossary](#glossary)
* [Team](#team)

## Problem Statement

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. 

## Objectives

The objective is to find the parameters that contribute the most in deciding the price of the house

## Data Understanding

The data provided has the data related to the house. It has categorical and numerical data.


## Data cleaning and manipulation

Data cleaning on columns - 
- Find all columns with all NULL values and replace it with default value or median.
- Correct the data type and standardise columns
- Add derived columns like houseAge
- Convert categorical data using dummies
- Convert data to be between 0 and 1 using MinMax scaler 

## Data Analysis

- Create OLS model to check the p-values
- Check the VIF values using the RFE
- Removed the columns with p-value >0.05 and VIF >5.
- Create a ridge object with different values of alpha. Consider the alpha to be 10
- Create a Lasso object and consider the alpha to be 100

## Conclusions
- Top predictors are - 'OverallQual','BsmtFinSF1','1stFlrSF','2ndFlrSF','MSZoning_RL'
- r2 score for train data is 80% and the same on test data is 80%
- The residual grap doesnt show any pattern. Also the residual histogram shows max at 0. SO the model is statistically signficant.

## Technologies Used
- [Python - Version 3.12.1](https://www.python.org/downloads/release/python-3121/)
- [numpy - Version 1.26.2](https://github.com/numpy)
- [pandas - Version 2.1.4](https://github.com/pandas-dev/pandas)
- [matplotlib - Version 3.8.2](https://github.com/matplotlib)
- [seaborn - Version 0.13.1](https://github.com/seaborn)
- [Jupyter Notebook - Version 7.0.6]()
- [JupyterLab - Version 4.0.9]()

## Team
* [Prachi Goliwadekar]
