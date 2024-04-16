# Module 12 Report Template

## Overview of the Analysis
**Description**
This analysis aims to leverage various machine learning techniques to train and evaluate the performance of Logistic Regression Models in identifying the creditworthiness of borrowers.This analysis aims to leverage various machine learning techniques to train and evaluate the performance of Logistic Regression Models in identifying the creditworthiness of borrowers.

In order to complete this process, I first seperated the existing 'loan_status' column (as the y variable) from the rest of the DataFrame (and made that the X variable). Next, I used the train_test_split module to create 'X_train', 'X_test', 'y_train' and 'y_test' values for the rest of the analysis. I then used the LogisticRegression module to create a 'classifier' variable that I used to fit the model using the training data. I made predicitons using the 'X-test' variable and then I evaluated the model's performance by generating a confusion matrix and a classification report.
## Results

Machine Learning Model 1:
  - Precision score for 0 (Healthy Loan) was 1.00 and for 1 (High-Risk Loan) was 0.87.
  - Recall score for 0 (Healthy Loan) was 1.00 and for 1 (High-Risk Loan) was 0.89.
  - Accuracy score for Precision was 0.94 (macro avg) and 0.99 (weighted avg).
  - Accuracy score for Recall was 0.94 (macro avg) and 0.99 (weighted avg).
  - The F1 Score for for 0 (Healthy Loan) was 1.00 and for 1 (High-Risk Loan) was 0.88.


## Summary

Based on the results from the machine learning model, you can see the model performs very well. I would recommend the usage by the company. While the model cannot predict a perfect 100% of the high-risk loans, it seems to be mostly maxed out with the accuracy score at 99%. In terms of predicting the high-risk loans, 89% is a strong percentage to capture the majority of these cases that can become financial strains on a loan provider if not properly identified during the loan application process. In other words, the company would be better off using the model and accepting the 89% success rate vs. not using the model at all.

Based on the result, for further learning, I may try to resample the data, by using RandomOverSampler module to solve the imbalanced classes issue.



