# credit-risk-classification

Attached please find the documents for the Module 20 Challenge within the 'Credit_Risk' folder:
  - The 'credit_risk_classification.ipynb' file which features the code for the Logistic Regression Model.
  - The 'Resources' folder which includes the 'lending_data.csv' file that was loaded in for analysis.

**Credit Risk Analysis Report**

Overview of the Analysis

The purpose of this project was to train and evaluate a model based on loan risk. The financial information at our disposal included loan size, interest rate, borrower income, a debt-to-income ratio, the number of accounts, any derogatory marks, and total debt. We used this information to predict a loan status of either 0 (healthy) or 1 (high-risk).

In order to complete this process, I first seperated the existing 'loan_status' column (as the y variable) from the rest of the DataFrame (and made that the X variable). Next, I used the train_test_split module to create 'X_train', 'X_test', 'y_train' and 'y_test' values for the rest of the analysis. I then used the LogisticRegression module to create a 'classifier' variable that I used to fit the model using the training data. I made predicitons using the 'X-test' variable and then I evaluated the model's performance by generating a confusion matrix and a classification report.

Results

Machine Learning Model 1:
  - Precision score for 0 (Healthy Loan) was 1.00 and for 1 (High-Risk Loan) was 0.87.
  - Recall score for 0 (Healthy Loan) was 1.00 and for 1 (High-Risk Loan) was 0.89.
  - Accuracy score for Precision was 0.94 (macro avg) and 0.99 (weighted avg).
  - Accuracy score for Recall was 0.94 (macro avg) and 0.99 (weighted avg).
  - The F1 Score for for 0 (Healthy Loan) was 1.00 and for 1 (High-Risk Loan) was 0.88.

Summary

To summarize all of the results from the model, the precision score of 1.00 (for healthy loans) and 0.87 (for high-risk loans) means that when the model predicts a loan as healthy or high-risk, it is right 100% and around 87% of the time respectively. For the recall scores, the value of 1.00 (for healthy loans) and 0.89 (for high-risk loans) indicates that the model correctly identified all of the healthy loans and the model captured 89% of the high-risk loans. The accuracy score measures the overall correctness of the model, so a value of 0.99 shows that 99% of the instances are correctly predicted.

Based on the results from the machine learning model, you can see the model performs very well. I would recommend the usage by the company. While the model cannot predict a perfect 100% of the high-risk loans, it seems to be mostly maxed out with the accuracy score at 99%. In terms of predicting the high-risk loans, 89% is a strong percentage to capture the majority of these cases that can become financial strains on a loan provider if not properly identified during the loan application process. In other words, the company would be better off using the model and accepting the 89% success rate vs. not using the model at all.
