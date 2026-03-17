# Telco Customer Churn Prediction

## Project Overview

Customer churn is one of the most critical challenges for subscription-based businesses such as telecommunications companies. Losing customers directly impacts revenue and increases the cost of acquiring new users.

This project develops a machine learning model to predict customer churn using historical customer data. By identifying customers at high risk of leaving, companies can implement targeted retention strategies and reduce customer attrition.

The project demonstrates an end-to-end data science workflow including data exploration, feature preprocessing, model training, evaluation, and interpretation of results.

---

## Dataset

The dataset contains customer-level information from a telecommunications service provider.

Key types of information included in the dataset:

- Customer demographics (gender, partner, dependents)
- Account information (tenure, contract type, billing method)
- Services subscribed (internet service, streaming, tech support, etc.)
- Financial data (monthly charges, total charges)
- Target variable: **Churn** (Yes/No)

Each row represents a customer and whether they eventually left the service.

---

## Business Problem

Customer acquisition is typically much more expensive than customer retention. Therefore, identifying customers who are likely to churn allows companies to take proactive measures such as:

- targeted promotions
- service improvements
- personalized retention offers

The objective of this project is to build a predictive model capable of identifying customers with a high probability of churn.

---

## Methodology

The project follows a structured machine learning workflow:

### 1. Data Exploration
Initial analysis to understand the structure of the dataset and identify patterns related to churn.

### 2. Data Cleaning
Handling data types, missing values, and preparing variables for modeling.

### 3. Exploratory Data Analysis (EDA)
Visualization and analysis of key variables such as tenure, monthly charges, contract type, and subscribed services to identify potential churn drivers.

### 4. Feature Preprocessing
A preprocessing pipeline is built using **scikit-learn**, including:

- missing value imputation
- feature scaling for numerical variables
- one-hot encoding for categorical variables

### 5. Model Training
Two classification models are trained and compared:

- Logistic Regression (baseline model)
- Random Forest Classifier

### 6. Model Evaluation
Models are evaluated using multiple classification metrics and visual diagnostics.

### 7. Feature Importance
Feature importance analysis is used to understand which variables contribute most to predicting churn.

### 8. Model Export
The final model is saved for future inference using **joblib**.

---

## Models

Two models were implemented:

### Logistic Regression
Used as a baseline interpretable model for binary classification.

### Random Forest Classifier
A tree-based ensemble model capable of capturing non-linear relationships and interactions between features.

---

## Evaluation Metrics

Model performance is evaluated using standard classification metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

These metrics help assess both overall performance and the model's ability to correctly identify customers who are likely to churn.

---

## Key Insights

Exploratory analysis and model interpretation highlight several important factors influencing churn:

- **Contract type** is one of the strongest predictors: customers with month-to-month contracts are significantly more likely to churn.
- **Tenure** plays a major role: customers with shorter relationships with the company show higher churn rates.
- **Monthly charges** show a relationship with churn probability.
- Additional services such as **tech support and online security** appear to reduce churn risk.

These insights can help guide customer retention strategies and service design decisions.

---

## Tech Stack

The project is implemented using the following tools:

- Python
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- joblib
