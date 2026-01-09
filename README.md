# Credit Risk Prediction Model

## Overview
This project focuses on building a **Credit Risk Prediction Model** to estimate the probability of loan default using customer demographic, financial, and credit behavior data. The model is designed to support **risk assessment and lending decision-making**.

An interactive **Streamlit web application** is used to demonstrate real-time predictions based on user inputs.

---

## Problem Statement
Financial institutions need to assess the likelihood of loan default before approving credit.  
The objective of this project is to:
- Predict **default probability**
- Generate a **credit score**
- Assign a **risk rating** (e.g., Good, Average, Poor)

---

## Dataset
The dataset contains customer-level loan and credit information, including:
- Demographics (age, dependents, residence duration)
- Loan details (loan amount, tenure, purpose, type)
- Credit behavior (delinquency, credit utilization, open/closed accounts)
- Target variable: **Default (0 = No, 1 = Yes)**

---

## Exploratory Data Analysis (EDA)
Key EDA steps performed:
- Distribution analysis of numerical features
- Comparison of default vs non-default customers
- Correlation analysis to identify relationships and multicollinearity
- Identification of strong predictors such as:
  - Loan tenure
  - Delinquency metrics
  - Credit utilization ratio
  - Loan-to-income ratio

Visualizations include:
- Histograms & KDE plots
- Correlation heatmap
- Class-wise distribution comparisons

---

## Model Building
Multiple models were trained and evaluated, including:
- Logistic Regression
- XGBoost (final selected model)

### Model Selection Criteria
- ROC–AUC score
- Precision–Recall tradeoff
- Ability to handle class imbalance

---

## Model Evaluation
The final model achieved strong performance:

- **ROC–AUC:** ~0.98  
- High recall for defaulters
- Stable performance across train and test sets

Evaluation techniques:
- Classification report
- ROC curve analysis
- AUC score comparison

---

## Deployment (Streamlit App)
The trained model is deployed using **Streamlit** to provide an interactive interface where users can:
- Enter applicant and loan details
- Instantly view:
  - Default probability
  - Credit score
  - Risk category

### Live Application
👉 https://credit-risk-predictions-model.streamlit.app/

---
