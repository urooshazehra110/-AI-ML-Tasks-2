# Customer Churn Prediction using Scikit-learn Pipeline

## Objective

The objective of this project is to build a reusable and production-ready machine learning pipeline for predicting customer churn in a telecommunications company.

The pipeline automates data preprocessing, model training, hyperparameter tuning, evaluation, and deployment.

---

## Dataset

Telco Customer Churn Dataset

The dataset contains customer demographic information, service subscriptions, billing information, and churn status.

Target Variable:

* Churn = 1 (Customer left)
* Churn = 0 (Customer retained)

---

## Methodology

### Data Cleaning

* Removed customerID
* Converted TotalCharges to numeric values
* Handled missing values

### Data Preprocessing

Implemented using Scikit-learn Pipeline API:

#### Numerical Features

* Missing value imputation
* Standard Scaling

#### Categorical Features

* Missing value imputation
* One-Hot Encoding

### Models

1. Logistic Regression
2. Random Forest Classifier

### Hyperparameter Tuning

GridSearchCV was used to identify optimal model parameters using cross-validation.

### Model Export

The final pipeline was exported using Joblib for future inference and deployment.

---

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score

---

## Results

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 80%  |
| Random Forest       | 79%  |

Logistic Regression generally provided better predictive performance.

---

## Technologies Used

* Python
* Scikit-learn
* Pandas
* NumPy
* Joblib
* Matplotlib
* Seaborn
