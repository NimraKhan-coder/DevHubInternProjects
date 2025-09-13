Telco Customer Churn Prediction
Overview

This project builds and evaluates machine learning models to predict customer churn in a telecommunications company. The dataset used is the Telco Customer Churn dataset from Kaggle, which includes customer demographics, account information, services subscribed, and churn labels.

The primary goal is to identify customers at risk of leaving the company, enabling proactive retention strategies.

Dataset

Source: Telco Customer Churn Dataset (Kaggle)

Size: ~7,000 customer records

Target Variable:

Churn (Yes/No → encoded as 1/0)

Key Features:

Customer demographics (gender, senior citizen, partner, dependents)

Account information (tenure, contract type, payment method, monthly charges, total charges)

Services subscribed (phone, internet, streaming, etc.)

Methodology

Data Preprocessing

Dropped irrelevant columns (customerID).

Converted TotalCharges to numeric, filled missing values with median.

Encoded target variable (Churn).

Train/test split (80/20).

Preprocessing pipeline using ColumnTransformer:

Standard scaling for numerical features.

One-hot encoding for categorical features.

Models Implemented

Logistic Regression (baseline model).

Random Forest Classifier (ensemble method).

Both integrated into pipelines with preprocessing.

Evaluation Metrics

Accuracy score.

Classification report (precision, recall, F1-score).

Model Saving

Trained models are saved using Joblib for reuse.

Results

Logistic Regression: Provides interpretable results and reasonable accuracy.

Random Forest: Achieves higher performance by capturing complex feature interactions.

Accuracy and F1-scores indicate that ensemble methods outperform baseline logistic regression.
