# credit-risk-classification

## Overview of the Analysis
The purpose of the analysis was to build and evaluate logistic regression models for predicting loan status (healthy loan or high-risk loan) using financial information. The data provided was on lending and contained features related to loans, and the target variable was the loan status.

The target variable, loan_status, had two distinct values:

0 representing healthy loans (low-risk)
1 representing high-risk loans
The analysis went through the following stages of the machine learning process:

Splitting the data into training and testing sets.
Creating a logistic regression model with the original data.
Evaluating the model's performance using accuracy, confusion matrix, and classification report.
Resampling the training data using the RandomOverSampler module to address class imbalance.
Creating another logistic regression model with the resampled data.
Evaluating the model's performance with the resampled data using accuracy, confusion matrix, and classification report.
The logistic regression models were used for classification, with the original data and resampled data to address class imbalance.

Results

Machine Learning Model 1: Logistic Regression Model with Original Data
Balanced Accuracy Score: 94%
Precision for High-Risk Loans (1): 87%
Precision for Healthy Loans (0): 100%
Machine Learning Model 2: Logistic Regression Model with Resampled Training Data
Balanced Accuracy Score: 100%
Precision for High-Risk Loans (1): 87%
Precision for Healthy Loans (0): 100%

Summary

Both logistic regression models performed well in terms of predicting healthy loans (0) with 100% precision. However, when it comes to predicting high-risk loans (1), both models had a precision of 87%.

In terms of overall performance, the logistic regression model trained with the resampled data showed a higher balanced accuracy score of 100% compared to the original data model with a balanced accuracy score of 94%. This indicates that the resampled model was better at correctly classifying both healthy and high-risk loans.

Considering the balanced accuracy score and precision, the logistic regression model with resampled training data is recommended for predicting loan status. It provides a more reliable performance overall, especially in handling class imbalance. However, it's important to note that performance evaluation should also consider the specific requirements and priorities of the problem at hand.
