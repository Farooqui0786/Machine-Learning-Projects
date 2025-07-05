# 📊 Customer Churn Prediction Using Machine Learning

This project aims to predict customer churn (i.e., whether a customer will leave or stay) using supervised machine learning techniques. The dataset is based on telecom customer data and includes both numerical and categorical features.

---

## 🔍 Problem Statement

Churn prediction is a common business problem in industries like telecom, banking, and SaaS. Retaining customers is more cost-effective than acquiring new ones. Using this model, businesses can proactively identify customers likely to leave and take retention actions.

---

## 📁 Dataset

- Source: Telco Customer Churn Dataset  
- File: `WA_Fn-UseC_-Telco-Customer-Churn.csv`  
- Columns include customer info like `gender`, `tenure`, `MonthlyCharges`, `TotalCharges`, and churn status (`Yes`/`No`).

---

## 🧠 Techniques Used

- Data Cleaning & Preprocessing
  - Handling missing and blank values
  - Label encoding for categorical features
  - Feature scaling (optional)
- Class Imbalance Handling
  - Applied **SMOTE** (Synthetic Minority Oversampling Technique)
- Model Building
  - **Decision Tree**
  - **Random Forest**
  - **XGBoost**
- Model Evaluation
  - Accuracy, Confusion Matrix, Classification Report
  - Cross-validation scores (5-fold)
- Model Saving & Reuse
  - Pickled `.pkl` files for model and encoders
  - Predictive interface for new data

---

## 📦 Files in This Repository

| File Name                          | Description                                         |
|-----------------------------------|-----------------------------------------------------|
| `Customer Churn Prediction.ipynb` | Complete Colab notebook with code and explanations |
| `WA_Fn-UseC_-Telco-Customer-Churn.csv` | Dataset used in the project                  |
| `label_encoders.pkl`              | Saved label encoders for categorical columns       |
| `customer_churn_model.pkl`        | Trained Random Forest model                        |
| `README.md`                       | Project documentation                              |

---

## 🚀 How to Run the Project

1. Clone the repo or download the files.
2. Open `Customer Churn Prediction.ipynb` in Jupyter/Colab.
3. Install required libraries (`scikit-learn`, `xgboost`, `imblearn`, etc.)
4. Run the notebook step-by-step.
5. Use the trained model to make predictions on new customer data.

---

## 📊 Sample Prediction Output

```python
Prediction: Churn
Prediction Probability: [[0.23, 0.77]]
