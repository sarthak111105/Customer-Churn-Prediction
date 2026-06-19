# Customer Churn Prediction in Telecom Using Machine Learning

## Project Overview
This project predicts customer churn in the telecom industry using Machine Learning. The goal is to identify customers who are likely to leave the service so that retention strategies can be applied proactively.

## Dataset
- Telco Customer Churn Dataset
- 7043 customer records
- 21 features
- Target Variable: Churn (Yes/No)

## Data Preprocessing
- Converted TotalCharges to numeric format
- Replaced missing values with 0
- Simplified "No internet service" and "No phone service" categories
- Encoded binary features (Yes=1, No=0)
- Created new features:
  - NumServices
  - TenureGroup

## Model Used
### CatBoost Classifier

- Handles categorical features efficiently
- Requires minimal preprocessing
- Reduces target leakage using ordered boosting
- Provides strong predictive performance

### Training Configuration
- Train-Test Split: 80%-20%
- Iterations: 1000
- Depth: 6
- Learning Rate: 0.1
- Class Weights applied for class imbalance

## Performance

| Metric | Value |
|----------|----------|
| Accuracy | 77% |
| ROC-AUC | 0.85 |

### Important Features
- Tenure
- Contract Type
- Monthly Charges

## Business Impact
- Early churn detection
- Reduced revenue loss
- Better customer retention
- Targeted customer engagement

## Future Innovation
### STAYO – Churn Prediction Bot

A future intelligent assistant that:
- Predicts churn risk
- Suggests personalized retention offers
- Automates customer engagement
- Continuously learns from customer behavior

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-Learn
- CatBoost
- Matplotlib
- Jupyter Notebook

## Authors
- Sarthak Sharma
- Shalin Sawhney
- Vaibhav Sharma
- Aastha Gupta
- Harnoor
