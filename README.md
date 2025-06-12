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

- **Logistic Regression** → baseline model  
- **Random Forest Classifier** → more powerful model

### 4. Evaluation Metrics

**Logistic Regression:**

- Accuracy: **65%**
- Precision: **0.0**
- Recall: **0.0**
- F1 Score: **0.0**

**Random Forest Classifier:**

- Accuracy: **65%**
- Precision: **1.0**
- Recall: **1%**
- F1 Score: **0.03**

### 5. Key Insights

- **MonthlyCharges** and **TotalCharges** are strong drivers of churn → pricing strategy is critical.
- **Tenure** is important → short-tenure customers more likely to churn → early retention programs needed.
- Demographics (Partner, Dependents) also influence churn behavior.

### 6. Model Limitations and Next Steps

- Models struggled with class imbalance → Recall for churn cases is low.
- Future improvements:
  - Apply **SMOTE** or class weighting to balance classes.
  - Tune classification threshold to improve churn recall.
  - Try advanced models such as **XGBoost** or **LightGBM**.
  - Explore additional feature engineering opportunities.

### 7. Business Recommendations

- Focus retention offers on customers with **high charges + short tenure**.
- Analyze pricing bundles and loyalty incentives.
- Develop onboarding programs targeting early churn reduction.
- Explore targeted marketing campaigns for segments with higher churn risk.

## Conclusion

This project demonstrates an end-to-end workflow for a classic business analytics problem:

- Data understanding and visualization
- Feature engineering and cleaning
- Modeling and evaluation
- Business-focused interpretation of results
- Recommendations for business action

