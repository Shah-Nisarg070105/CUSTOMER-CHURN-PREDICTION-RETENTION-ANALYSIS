# 📊 Customer Churn Prediction & Retention Analysis

## 🚀 Project Overview
Customer churn is a major challenge for telecom companies, directly impacting revenue and growth.  
This project builds an **end-to-end churn prediction system** using machine learning, with a focus on **business impact and decision-making** rather than just model accuracy.

The goal is to:
- Identify customers likely to churn  
- Understand key drivers of churn  
- Provide actionable strategies for customer retention  

---

## 🎯 Key Features
- End-to-end ML pipeline (data cleaning → modeling → evaluation)
- Feature engineering based on customer behavior
- Model optimization using cross-validation and hyperparameter tuning
- Threshold tuning to maximize business impact
- Model explainability using feature importance and SHAP

---

## 🛠️ Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, SHAP  
- **Concepts:** Machine Learning, Feature Engineering, Model Evaluation, Cross-Validation, Threshold Optimization  

---

## 📦 Dataset
- Telco Customer Churn Dataset (Kaggle)
- Contains customer demographics, services, billing, and churn status

---

## 🧹 Data Preprocessing
- Handled missing values and converted data types (e.g., `TotalCharges`)
- Encoded categorical variables using one-hot encoding
- Removed multicollinearity (dummy variable trap)
- Cleaned and standardized dataset for modeling

---

## 🧠 Feature Engineering
Created meaningful features to improve model performance:
- **Approximate Tenure** (from tenure groups)
- **Average Monthly Spend**
- **Total Services Used**

---

## 🤖 Models Used
- Logistic Regression (baseline model)
- Random Forest (non-linear model)

---

## 📊 Model Evaluation

| Metric | Logistic Regression | Random Forest |
|-------|---------------------|--------------|
| Accuracy | ~73% | ~78% |
| Precision | ~49% | ~61% |
| Recall | ~78% → **93% (after tuning)** | ~49% |

👉 Final model optimized for **high recall (~93%)** to minimize missed churn customers.

---

## 🎯 Threshold Optimization
Instead of using the default threshold (0.5), it was tuned to **0.3** to:
- Increase recall significantly  
- Reduce missed churn cases  
- Align model with real-world business needs  

---

## 🔍 Key Insights
- Customers with **low tenure** are more likely to churn  
- **Higher monthly charges** increase churn probability  
- **Month-to-month contracts** show highest churn rates  
- **Electronic payment methods** are associated with higher churn  

---

## 💼 Business Recommendations
- Improve onboarding experience for new customers  
- Offer incentives for long-term contracts  
- Provide targeted discounts for high-risk customers  
- Improve payment experience for electronic methods  

---

## 🔎 Model Explainability
- Feature importance analysis identified key churn drivers  
- SHAP used to explain model predictions and feature impact  

---

## ⚠️ Limitations
- Approximate tenure is derived using midpoint estimation  
- Some features (e.g., TotalCharges) are highly correlated with others  
- Further feature engineering and tuning can improve performance  

---

## 📸 Sample Outputs
(Add screenshots here: confusion matrix, feature importance, etc.)

---

## 📌 Conclusion
This project demonstrates how machine learning can be applied to solve real-world business problems by focusing on:
- **Impact over accuracy**
- **Interpretability**
- **Data-driven decision making**

---

## 🔗 Future Improvements
- Deploy as a Streamlit web application  
- Integrate real-time prediction system  
- Use advanced models like XGBoost  

---

## 🙌 Acknowledgment
Dataset sourced from Kaggle (Telco Customer Churn Dataset)

---

## 📬 Contact
If you found this project interesting or have feedback, feel free to connect!
