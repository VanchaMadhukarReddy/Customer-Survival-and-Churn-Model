# Customer Churn Prediction & Survival Analysis

This project focuses on understanding why customers leave a service (churn) and predicting the likelihood of churn using machine learning and survival analysis. It also includes a Flask web application that visualizes churn risk, survival probability, and key model explanations.

## 🚀 Project Overview

Customer churn is one of the most important challenges for subscription-based businesses such as telecom, internet providers, insurance, and streaming services. Retaining an existing customer costs far less than acquiring a new one.

This project combines:

- Exploratory Data Analysis (EDA)
- Survival Analysis (Kaplan–Meier, Log-Rank, Cox Model)
- Machine Learning (Random Forest)
- Explainability (SHAP Values, Permutation Importance, PDP)
- Flask Web Application

The goal is to estimate:

- How churn risk changes over time
- Which customer features influence churn
- A customer’s expected lifetime value
- Whether a specific customer is at high or low churn risk

---

## 🏗️ Project Structure

├── Images/
├── static/ # Plots for survival curve, hazard curve & SHAP values
├── templates/ # HTML templates for Flask app
├── Exploratory Data Analysis.ipynb
├── Customer Survival Analysis.ipynb
├── Churn Prediction Model.ipynb
├── app.py # Flask web application
├── model.pkl # Trained Random Forest model
├── survivemodel.pkl # Cox-Proportional Hazard model
├── explainer.bz2 # SHAP explainer
├── requirements.txt
└── README.md

---

## 📊 Survival Analysis

Survival analysis helps estimate how long a customer is likely to stay subscribed.  
The project uses:

### **📌 Kaplan–Meier Curve**

Shows how customer survival probability changes over time.

### **📌 Log-Rank Test**

Compares churn survival between different customer groups (internet type, contract type, payment method, etc.).

### **📌 Cox-Proportional Hazard Model**

Identifies which features increase or reduce churn risk.

Using this model, the app can calculate:

- Survival curve for any customer
- Hazard curve
- Expected remaining lifetime
- Estimated customer lifetime value (LTV)

---

## 🤖 Machine Learning (Churn Prediction Model)

A Random Forest classifier was trained with:

- Class balancing (handling churn imbalance)
- GridSearchCV hyperparameter tuning
- 80/20 train-test split without data leakage

**Final Performance:**

- **F1 Score:** ~0.62
- **ROC–AUC:** ~0.85

### 🔍 Explainability Tools Used

- **Permutation Importance**
- **Partial Dependence Plots**
- **SHAP Values**

These tools help understand _why_ the model predicts churn for a specific customer.

---

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- Lifelines (Survival Analysis)
- Matplotlib, Seaborn
- Flask
- SHAP
- HTML/CSS

---

## 👨‍💻 Author

**Vancha Madhukar Reddy**  
Machine Learning & Full-Stack Developer  
LinkedIn: _your_link_here_

---
