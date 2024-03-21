# Module 12 Report

## Overview of the Analysis

### Purpose of the Analysis
The primary purpose of this analysis was to leverage machine learning techniques to predict the likelihood of a loan being high-risk (1) or healthy (0). By doing so, financial institutions can identify potential default risks before issuing loans, enhancing their risk management frameworks and ensuring financial stability.

### Financial Information
The dataset used in this analysis, lending_data.csv, contained financial information about borrowers, including:

- Loan size
- Interest rate
- Borrower income
- Debt-to-income ratio
- Number of accounts
- Derogatory marks
- Total debt
- Loan status (the target variable to predict, indicating healthy or high-risk loans)

### Stages of the Machine Learning Process
The machine learning process for this analysis involved several stages:

- Data Preparation: Loading the dataset and splitting it into features (X) and the target variable (y).
- Splitting the Data: Dividing the dataset into training and testing sets to evaluate the model's performance on unseen data.
- Model Training: Using the LogisticRegression algorithm from sklearn to train the model on the training data.
- Model Evaluation: Predicting the loan status on the test dataset and evaluating the model's performance using metrics such as accuracy, precision, recall, and the F1-score, provided through a confusion matrix and classification report.

### Methods Used
The primary method used in this analysis was Logistic Regression, chosen for its effectiveness in binary classification problems, simplicity, and interpretability. Logistic regression is particularly suitable for predicting binary outcomes, making it an excellent choice for classifying loans as either high-risk or healthy based on the borrower's financial information.

Through the logistic regression model, we achieved high accuracy, with precision and recall metrics indicating that the model was effective in identifying both healthy and high-risk loans. This suggests that logistic regression, combined with a well-prepared dataset, can be a powerful tool for credit risk assessment in the financial sector.

## Results

### Machine Learning Model 1: Logistic Regression

Accuracy:
* Overall accuracy of the model is 0.99, indicating that it correctly predicts the loan status 99% of the time across both categories (healthy and high-risk loans).

Precision:
* Precision for predicting healthy loans (0): 1.00, meaning there were no healthy loans incorrectly classified as high-risk.
* Precision for predicting high-risk loans (1): 0.85, indicating that 85% of loans predicted as high-risk were actually high-risk.

Recall:
* Recall for healthy loans (0): 0.99, suggesting that the model identified 99% of all actual healthy loans correctly.
* Recall for high-risk loans (1): 0.95, indicating that the model identified 95% of all actual high-risk loans correctly.

## Summary

These metrics reveal that the Logistic Regression model performed exceptionally well in predicting both healthy and high-risk loans. The high precision and recall scores for both categories show that the model is not only accurate overall but also effectively balances the ability to identify true positives without significantly increasing false positives, especially important for high-risk loan predictions in financial applications.
