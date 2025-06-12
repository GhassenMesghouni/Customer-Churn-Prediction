# Customer Churn Prediction

## Project Overview

This project predicts customer churn using machine learning models based on simulated Telco customer data.

Customer churn is a key business problem in subscription-based industries. Reducing churn has direct impact on revenue and customer lifetime value. The goal is to build models that help identify at-risk customers so the business can take proactive retention actions.

## Dataset

- 1000 simulated Telco customer records
- Features include: demographics, services, tenure, billing information
- Target variable: **Churn** (Yes/No)

## Process

### 1. Exploratory Data Analysis (EDA)

- Distribution of key features
- Relationship between features and churn
- Handling missing values and data types

### 2. Data Cleaning and Preprocessing

- Converted categorical variables to numerical format
- One-hot encoding for multi-category variables
- Scaling of features where necessary

### 3. Modeling

- Logistic Regression → baseline model
- Random Forest Classifier → more powerful model

### 4. Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Feature Importance (Random Forest)

### 5. Key Insights

- **MonthlyCharges** and **TotalCharges** are strong drivers of churn → pricing strategy is critical.
- **Tenure** is important → short-tenure customers more likely to churn → early retention programs needed.
- Demographics (Partner, Dependents) also influence churn behavior.

### 6. Model Limitations and Next Steps

- Models struggled with class imbalance → Recall for churn cases is low.
- Future improvements:
  - Apply **SMOTE** or class weighting.
  - Tune classification threshold.
  - Try advanced models (XGBoost, LightGBM).

### 7. Business Recommendations

- Focus retention offers on customers with **high charges + short tenure**.
- Analyze pricing bundles and loyalty incentives.
- Develop onboarding programs targeting early churn reduction.

## Conclusion

This project demonstrates an end-to-end workflow for a classic business analytics problem:

- Data understanding
- Feature engineering
- Modeling and evaluation
- Business-focused interpretation

