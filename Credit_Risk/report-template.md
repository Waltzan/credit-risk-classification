# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Credit Risk Analysis
The purpose of this analysis is to predict the possiblity of customers who may default on their loans. This is based on a lending data received in a csv format, which was used to predict the data with machine learning and python. The lending data contained loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt and loan status data. The loan status column is the data I was trying to predict by using logistic regression model by importing "from sklearn.linear_model import LogisticRegression" to determine the trend for '0'(healthy loan) and '1'(high-risk loan) labels. The process started with importing the necesary modules; numpy as np, os, pandas as pd, from pathlib import path, from sklearn.metrics import confusion_matrix and classification _report. To split the data into training and testing sets; the lending data csv was read in as a pandas DataFrame, then the labels and features were separated creating a y and x variable. Then the data was split using module "from sklearn.model_selection import train_test_split" after which the logistic regression model was created, using the model, fit, predit method. Lastly, the model's performance was evaluated using the confusion matrix and classification reports.
    In the classification reports, the training report had;
    