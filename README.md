# MapReduce

Implement MapReduce in Python for processing and generating large data sets with a parallel and distributed algorithm on a cluster.

Key features:

- MapReduce
- Exploratory data analysis (EDA)

Modules used:

- `os`: a portable way of using operating system dependent functionality
- `functools`: higher-order functions that work on other functions
- `collections`: specialized container datatypes providing alternatives to Python’s general purpose built-in containers, dict, list, set, and tuple.
- `numpy`: Python library used for working with arrays
- `pandas`: data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.

## Project Report

[Project report](https://htmlpreview.github.io/?https://raw.githubusercontent.com/chsueh2/Online_Shoppers_Purchasing_Intention/main/online_shoppers.html) ([Jupyter Notebook](./MapReduce.ipynb))

The analysis results with theoretical backgrounds are included.

Chien-Lan Hsueh (chienlan.hsueh at gmail.com)

## Overview and Project Goal

Conduct EDA on the training set through spark SQL to get a good understanding of the data structure. This helps identify the useful predictors to be included in the models.

- For numeric variables: inspect collinearity and determine which to include in logistic regression
- For categorical variables: recode the variable if the data distribution is imbalanced

Fit machine learning models including logistic regression and two tree-based classification models (decision tree classifier and random forest classifier) using area under ROC curve as our model selection metric (evaluator).

## Workflow

1. Split data
2. MapReduce Implementation
   - Mapping Function
   - Reducer Function
3. EDA on NFL data using MapReduce
   - Mean and standard deviation of "AQ1" by "week"
   - Mean and standard deviation of "homeRushYds" by "day"
   - Mean and standard deviation of "homeRushYds" by "surface"
   - Mean and standard deviation of "HFinal" by "homeTeam"