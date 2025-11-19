# 📊 Telco Customer Churn Prediction | Machine Learning Project

This project analyzes the **Telco Customer Churn Dataset** and builds a machine learning model to predict whether a customer will churn (leave the service).  
The workflow includes **data cleaning, feature engineering, encoding, scaling, modeling, and evaluation**.

---

## 🚀 Project Objectives

- Understand customer churn behavior.
- Perform end-to-end data preprocessing.
- Handle categorical & numerical features properly.
- Build and evaluate a predictive ML model.
- Identify important features that influence churn.

---

## 📁 Dataset Details

**File:** `WA_Fn-UseC_-Telco-Customer-Churn.csv`  
**Rows:** 7,043  
**Columns:** 21  

### Key Features:
- Customer demographics  
- Contract types  
- Internet & phone service details  
- Monthly & total charges  
- Churn (target variable)

---

## 🧹 Data Preprocessing Steps

- Removed irrelevant columns (`customerID`)
- Handled missing values in `TotalCharges`
- Converted `TotalCharges` to numeric
- Encoded:
  - Binary categorical columns using **LabelEncoder**
  - Multi-category columns using **OneHotEncoding**
- Scaled numerical features using **StandardScaler**

---

## ⚙️ Model Used

### **Random Forest Classifier**
Chosen because:
- Works well with mixed feature types  
- Handles non-linear relationships  
- Resistant to overfitting  

---

## 📈 Model Performance

| Metric              | Score |
|---------------------|--------|
| **Accuracy**        | ~79%   |
| **Precision**       | Good for majority class |
| **Recall (Churn)**  | ~0.58 |
| **F1 (Churn)**      | ~0.67 |

### Confusion Matrix:
[[197,20], [79,108]
### Key Insight:
The model performs well on non-churn customers but moderately on churn customers — which is typical for this dataset.

---

## 🔥 Feature Importance

The top factors influencing churn:
- Contract type  
- Tenure  
- MonthlyCharges  
- InternetService (Fiber Optic)  
- OnlineSecurity  
- TechSupport  

---

## 🗂️ Project Files

- `notebook.ipynb` → Full code and analysis  
- `churn_model.pkl` → Saved Random Forest model  
- `scaler.pkl` → Saved StandardScaler  
- `README.md` → Project documentation  

---

## 🧠 What I Learned

- Real-world categorical encoding  
- Handling numerical conversion issues  
- Feature engineering best practices  
- Machine learning workflow end-to-end  
- Evaluating imbalanced classification problems  

---

## 📬 Contact
If you want help improving the project or deploying it, feel free to ask.

---
