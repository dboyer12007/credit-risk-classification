# Module 12 Report

## Overview of the Analysis

Purpose:
The analysis aims to predict whether a loan is healthy (label 0) or high-risk (label 1) using a machine learning model.

Data Description:
The dataset includes financial details about loans, such as repayment histories, and the goal is to classify loans based on their risk. There is a noticeable imbalance in the data, with 18,765 healthy loans and only 619 high-risk loans.

Process Overview:
The features and target labels were assigned to X and y variables, and the data was split into training and testing datasets. After training, the predicted values were evaluated using a confusion matrix to determine the number of false positives and false negatives. A classification report was then generated to assess the performance of the logistic regression model.

Methods:
The LogisticRegression algorithm was used as the baseline model for this analysis.



## Results

Logistic Regression:

Accuracy: 99%
Precision (healthy loans): 1.00
Recall (healthy loans): 0.99
F1-score (healthy loans): 1.00
Precision (high-risk loans): 0.85
Recall (high-risk loans): 0.95
F1-score (high-risk loans): 0.89
Precision (macro): 0.92
Recall (macro): 0.97
F1 (macro): 0.94
Precision (weighted): 0.99
Recall (weighted): 0.99
F1-score (weighted): 0.99

## Summary

The logistic regression model achieved an overall accuracy of 99%, demonstrating strong performance on healthy loans (0) but showing some limitations on high-risk loans (1). While the model is 100% accurate in predicting healthy loans, it is only 85% precise in identifying high-risk loans, with a recall of 95% and an F1-score of 0.89.

This imbalance could lead to financial risks, as misclassifying high-risk loans (false negatives) may result in significant liabilities. The disparity in the dataset—18,765 healthy loans versus 619 high-risk loans—likely contributes to this issue.

Machine learning algorithms often prioritize the majority class to minimize overall error, which can result in underperformance on the minority class. To address this imbalance, techniques such as oversampling the minority class, class weighting, or using advanced algorithms like Random Forest or Gradient Boosting could be employed. These methods may improve the model’s ability to identify high-risk loans and reduce potential financial losses.
