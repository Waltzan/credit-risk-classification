# credit-risk-classification

Credit risk classification Analysis
The purpose of this analysis is to predict the possibility of customers who may default on their loans. This is based on lending data received in a csv format, which was used to predict the data with machine learning and python. The lending data contained loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt and loan status data. The loan status column is the data I was trying to predict by using logistic regression model by importing "from sklearn.linear_model import LogisticRegression" to determine the trend for '0'(healthy loan) and '1'(high-risk loan) labels. The process started with importing the necessary modules; NumPy as np, OS, pandas as pd, from pathlib import path, from sklearn.metrics import confusion matrix and classification _report. To split the data into training and testing sets; the lending data csv was read in as a pandas DataFrame, then the labels and features were separated creating a y and x variable. Then the data was split using module "from sklearn.model_selection import train_test_split" after which the logistic regression model was created, using the model, fit, predict method. Lastly, the model's performance was evaluated using the confusion matrix and classification reports.
Results
    The training classification report had the following for ‘0’ – healthy loans:
a)	Precision at 1.00 (100%)
b)	Recall at 1.00 (100%)
c)	Accuracy at 0.99 (99%)
  The testing classification report had the following for ‘0’ - healthy loans:
a)	Precision at 1.00 (100%)
b)	Recall at 0.99 (99%)
c)	Accuracy at 0.99 (99%)
   The training classification report had the following for ‘1’ – high risk loans:
a)	Precision at 0.86 (86%)
b)	Recall at 0.90 (90%)
c)	Accuracy at 0.99 (99%)
  The testing classification report had the following for ‘1’ – high risk loans:
a)	Precision at 0.85 (85%)
b)	Recall at 0.91 (91%)
c)	Accuracy at 0.99 (99%)
Precision measures the proportion of predicted positive values out of all instances predicted as positive. If the precision is high for ‘healthy loan’ then the model is good at correctly predicting healthy loans.
Recall measures the proportion of correctly predicted instances out of all the actual positive instances and so if the recall is high for healthy loan, this indicates the model is good at recognizing most of the healthy loan.
Confusion matrix provides tabular data of the model’s predictions against the actual labels showing true positives and negatives, and false positives and false negatives.
Summary
The machine learning models support data of healthy loans 18765 and high-risk loans at 619 in the testing classification report is slightly lower than the training classification report, which is normal to expect, since testing data performs relatively well in real life if it has a good precision and recall score. We can use this report to classify the credit risk and loan status because once we have trained our model well then testing it should be successful, and it is very useful to predict the “high-risk loans” since this would be the category of concern when it comes to find a solution for customers who may default on loans in the future.
    
