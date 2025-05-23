# 📊 Customer Churn Analysis and Prediction

This project aims to analyze and predict customer churn using a machine learning model based on a Telco customer dataset. The goal is to identify customers likely to leave the service, enabling better retention strategies.

---

## ✅ Objectives

1. Data preparation and cleaning
2. Feature selection
3. Model building (Random Forest)
4. Model evaluation
5. Insight visualization

---

## 🛠️ Main Project Steps

### 1. Data Preparation

- Remove rows with missing values in the target column Churn.
- Transform the target: Yes → 1, No → 0.
- Select relevant explanatory variables.
- Identify categorical and numerical columns.
- Preprocessing:
    - Impute missing numerical values with the most frequent value.
    - Impute missing categorical values and apply one-hot encoding.

### 2. Data Splitting

- Split the dataset into training (80%) and validation (20%) sets.

### 3. Feature Selection

- Manually select influential variables:
  `['gender', 'SeniorCitizen', 'Partner', 'Dependents', 'PhoneService', 'MultipleLines', 'InternetService', 'Contract', 'MonthlyCharges', 'tenure']`
- Analyze correlation between numerical variables.

### 4. Model Building

- Model: Random Forest Classifier (100 trees, random_state=42).
- Pipeline combining preprocessing and model.
- Train on the training set.

