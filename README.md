# credit-risk-classification

-------Overview of the Analysis

The purpose of this analysis was to evaluate the effectiveness of machine learning models in predicting loan status, specifically identifying healthy loans (0) and high-risk loans (1). The dataset contained financial information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The primary objective was to predict whether a loan falls into the high-risk category (loan_status = 1).

We first explored the dataset to understand its structure and distribution, including using value_counts to examine the balance of loan statuses. The machine learning process followed key steps: data preprocessing, splitting data into training and testing sets, training a logistic regression model, making predictions, and evaluating performance using accuracy, precision, recall, and a confusion matrix. The primary model used in this analysis was Logistic Regression, which is effective for binary classification tasks like this one.

----------Results

Machine Learning Model 1: Logistic Regression

Accuracy: 99%

Precision:

Healthy Loans (0): 100%

High-Risk Loans (1): 85%

Recall:

Healthy Loans (0): 99%

High-Risk Loans (1): 91%

F1-score:

Healthy Loans (0): 1.00

High-Risk Loans (1): 0.88

----------Summary

The logistic regression model performed exceptionally well, achieving a 99% accuracy rate. It predicted healthy loans (0) with near-perfect precision and recall, making very few misclassifications. However, its ability to detect high-risk loans (1) was slightly weaker, with an 85% precision and 91% recall, meaning some high-risk loans were misclassified as healthy.

If the goal is to minimize false negatives (i.e., avoid misclassifying high-risk loans as healthy), improvements such as handling class imbalance, using different algorithms (e.g., Random Forest or Gradient Boosting), or tuning hyperparameters might be beneficial. However, if overall accuracy is the key concern, logistic regression provides a strong baseline model. Based on this analysis, logistic regression is a viable model, but further refinement is recommended if identifying high-risk loans is the top priority.