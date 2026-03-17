# Telco Customer Churn Prediction

## Project Overview
This project predicts customer churn for a telecom company using machine learning.  
The goal is to identify customers likely to leave the service, helping the business take preventive actions.

## Dataset
The dataset contains customer demographic information, subscription details, account information, and churn labels.

## Business Goal
Reduce customer attrition by identifying high-risk customers and understanding key churn drivers.

## Main Steps
- Data loading and inspection
- Data cleaning
- Exploratory Data Analysis (EDA)
- Preprocessing with pipelines
- Logistic Regression baseline
- Random Forest model
- Model evaluation
- Feature importance
- Model export

## Models Used
- Logistic Regression
- Random Forest Classifier

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

## Key Insights
- Contract type strongly affects churn risk
- Customers with shorter tenure are more likely to churn
- Monthly charges have a relationship with churn behavior
- Some service-related features are important churn predictors

## Tech Stack
- Python
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- joblib
