# Financial Fraud Detection using Machine Learning

## Overview

This project focuses on building a machine learning model to detect fraudulent financial transactions. The dataset contains over 6 million transaction records including information such as transaction type, transaction amount, and account balances. The objective is to identify suspicious patterns and develop a predictive model that can detect fraudulent transactions effectively.

The project includes data cleaning, exploratory data analysis, model development, performance evaluation, and recommendations for fraud prevention strategies.

---

## Dataset
data set can be found here:  https://drive.google.com/uc?export=download&confirm=6gh6&id=1VNpyNkGxHdskfdTNRSjjyNa5qC9u0JyV
  
The dataset contains 6,362,620 transactions with the following features:

* step: Unit of time in hours
* type: Type of transaction (PAYMENT, TRANSFER, CASH_OUT, etc.)
* amount: Transaction amount
* nameOrig: Sender account ID
* oldbalanceOrg: Sender balance before transaction
* newbalanceOrig: Sender balance after transaction
* nameDest: Receiver account ID
* oldbalanceDest: Receiver balance before transaction
* newbalanceDest: Receiver balance after transaction
* isFraud: Fraud label (1 = Fraud, 0 = Legitimate)
* isFlaggedFraud: Flag for large suspicious transfers

---

## Project Workflow

The project follows a structured machine learning pipeline:

1. Data Loading
2. Data Cleaning
3. Exploratory Data Analysis
4. Feature Selection
5. Model Training
6. Model Evaluation
7. Fraud Pattern Analysis
8. Fraud Prevention Recommendations

---

## Data Cleaning

Data preprocessing steps include:

* Checking for missing values
* Removing irrelevant variables such as account identifiers
* Encoding categorical variables
* Detecting outliers in transaction amounts
* Checking correlations between variables to avoid multicollinearity

---

## Fraud Detection Model

A Random Forest Classifier was used to build the fraud detection model. Random Forest was selected because it handles large datasets effectively and can capture complex relationships between variables.

The model was trained on the training dataset and evaluated on the testing dataset.

---

## Model Evaluation

The performance of the model was evaluated using several metrics:

* Confusion Matrix
* Precision
* Recall
* F1 Score
* ROC-AUC Score

Since fraud datasets are highly imbalanced, recall and precision were considered more reliable indicators than accuracy.

---

## Key Factors Predicting Fraud

Feature importance analysis revealed that the following variables strongly influence fraud detection:

* Transaction amount
* Transaction type
* Sender account balance before transaction
* Sender account balance after transaction
* Receiver account balance changes

These variables capture abnormal financial behavior patterns.

---

## Fraud Prevention Strategies

Based on the analysis, financial institutions should implement the following measures:

* Real-time transaction monitoring systems
* Machine learning-based fraud detection
* Multi-factor authentication for high-risk transactions
* Transaction amount limits
* Behavioral analysis of account activity

---

## Measuring System Effectiveness

To determine whether the fraud detection system is effective, organizations should monitor:

* Reduction in fraud-related financial losses
* Fraud detection rate
* False positive rate
* Performance of the model over time

Continuous monitoring and periodic retraining of the model can help maintain system performance.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook



---

## Conclusion

This project demonstrates how machine learning techniques can be used to identify fraudulent financial transactions. The developed model successfully identifies patterns associated with fraud and provides insights that can help financial institutions improve their fraud detection systems.
