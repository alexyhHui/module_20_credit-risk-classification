# module_20_credit-risk-classification

## Credit Risk Analysis Report
## Overview of the Analysis

### Purpose of the Analysis
The purpose of this analysis is to develop and evaluate machine learning models for credit risk analysis. The goal is to predict whether a loan is healthy or high-risk based on financial information provided in the dataset.

### Financial Information and Prediction Target
The dataset contains information on various financial attributes of loans, such as loan size, interest rate and borrower income. The target variable is the loan status, which has two classes: healthy (0) and high-risk (1). The analysis aims to predict the loan status based on the given financial features.

### Basic Information about the Variables
`loan_status`:
Value counts:
- Healthy (0): 75036 instances
- High-risk (1): 2500 instances

### Stages of the Machine Learning Process
1. Data Preprocessing: Cleaning the dataset, handling missing values, encoding categorical variables, and splitting the data into training and testing sets.
2. Model Selection: Choosing appropriate machine learning algorithms for classification tasks. In this analysis, logistic regression is used due to its interpretability and effectiveness for binary classification.
3. Model Training: Training the logistic regression model using the training dataset.
4. Model Evaluation: Evaluating the trained model's performance using various metrics such as accuracy, precision, recall, F1-score, and balanced accuracy.

### Methods Used
- Logistic Regression: Employed for binary classification, given its interpretability and suitability for credit risk analysis.
- Resampling: In one scenario, oversampling technique was used to address class imbalance, ensuring equal representation of both classes in the training data.

## Results
Logistic Regression Model with Standard Data:

- Accuracy: 99%
- Precision for healthy loans: 100%
- Precision for high-risk loans: 85%
- Recall for healthy loans: 99%
- Recall for high-risk loans: 91%
- Balanced accuracy score: 95.2%

  
Logistic Regression Model with Oversampled Data:

- Accuracy: 99%
- Precision for healthy loans: 100%
- Precision for high-risk loans: 84%
- Recall for healthy loans: 99%
- Recall for high-risk loans: 99%
- Balanced accuracy score: 99.4%


## Summary
Both machine learning models demonstrate high accuracy in predicting credit risk, with an accuracy rate of 99% for both models. However, when comparing the precision and recall scores, the logistic regression model trained on oversampled data performs better than the model trained on standard data. The oversampled model achieves a balanced accuracy score of 99.4%, indicating superior performance in classifying both healthy and high-risk loans.

Given its higher precision and recall scores, as well as the significantly improved balanced accuracy, the logistic regression model trained on oversampled data is recommended for use by the company. This model provides more reliable predictions of credit risk, which is crucial for making informed lending decisions. The oversampling technique effectively mitigates class imbalance issues, resulting in a more robust and reliable predictive model.

In conclusion, the logistic regression model trained on oversampled data is the preferred choice for credit risk analysis due to its superior performance metrics and ability to provide more accurate predictions of creditworthiness.
