# 📊 Customer Churn Analysis & Prediction

An end-to-end **Customer Churn Analytics and Prediction** project built using  
**SQL Server, Python (Machine Learning), and Power BI** to identify churn drivers, predict high-risk customers, and support data-driven retention strategies.

---

## 🚀 Project Overview

Customer churn is one of the biggest challenges for subscription-based businesses.  
This project focuses on:

- Understanding customer churn behavior  
- Identifying key factors driving churn  
- Predicting customers likely to churn  
- Visualizing insights using interactive dashboards  

The project follows a **complete analytics lifecycle**, from raw data processing to business-ready insights.

---

## 🧱 Tech Stack

- **SQL Server** – Data cleaning, transformation, views  
- **Python** – Data preprocessing & ML model training  
- **Machine Learning** – Random Forest Classifier  
- **Power BI** – Interactive dashboards & reporting  
- **Jupyter Notebook** – Model development & evaluation  

---

## 🗂️ Data Architecture

### 🔹 Tables
- `stg_Churn` → Raw staging data  
- `prod_Churn` → Cleaned production data  

### 🔹 Views
- `vw_ChurnData` → Customers who *Stayed* or *Churned*  
- `vw_JoinData` → Newly *Joined* customers (used for prediction)  

---

## 🧹 Data Cleaning & Transformation (SQL)

- Replaced NULL values with business-friendly defaults  
- Standardized categorical columns  
- Created production-ready tables  
- Built views for analytics and ML pipelines  

### Example:

```sql
ISNULL(Internet_Type, 'None') AS Internet_Type,
ISNULL(Churn_Reason, 'Others') AS Churn_Reason
```

---

## 🌐 Live Power BI Dashboard

🔗 **View Live Dashboard:**  
https://app.powerbi.com/view?r=eyJrIjoiZTc5YTNjYTItYmJiMi00NzE2LThjZGUtOTNkMGJkNzIxMDUzIiwidCI6IjE5MjA4NDBiLTA0YjctNDRhZi05YTRkLTk4YmFkZjRlY2M0YSJ9

---

## 📈 Exploratory Data Analysis (EDA)

Performed analysis to understand:

- Gender-wise churn  
- Age group vs churn rate  
- State-wise churn (Top 5)  
- Contract & payment method impact  
- Revenue contribution by churn status  

---

## 🤖 Machine Learning Model

- **Algorithm:** Random Forest Classifier  
- **Target Variable:** `Customer_Status`  
  - Stayed → 0  
  - Churned → 1  
- **Train-Test Split:** 80% / 20%  
- **Model Accuracy:** ~84%  

### 🔍 Feature Importance (Top Drivers)

- Contract Type  
- Total Revenue  
- Monthly Charges  
- Tenure in Months  
- Internet Type  

---

## 🔮 Churn Prediction on New Customers

- Applied trained model on newly joined customers  
- Identified customers at high risk of churn  
- Exported predicted churn data for Power BI reporting  

---

## 📊 Power BI Dashboards

### 🔹 Churn Summary Dashboard

Includes:
- Total Customers  
- New Joiners  
- Churn Rate  
- Total Churn  
- Churn by Gender, Age, and State  
- Churn by Contract & Payment Method  
- Services vs Churn  

---

### 🔹 Churn Prediction Dashboard

Includes:
- Predicted churners count  
- High-risk customer profiles  
- State-wise churn risk  
- Contract & payment method impact  
- Customers-at-risk table  

---

## 💡 Business Impact

This project enables organizations to:

- Identify churn-prone customers early  
- Reduce potential revenue loss  
- Design targeted retention strategies  
- Improve customer lifetime value (CLV)  

---

## ✅ Key Learnings

- End-to-end data analytics workflow  
- SQL-based data engineering  
- Machine learning model development  
- Business-focused dashboard design  
- Translating data into actionable insights  

---

## 📌 Future Improvements

- Hyperparameter tuning  
- SHAP-based model explainability  
- Real-time churn prediction  
- Automated data pipelines  

---

## 👤 Author

**Sumit Bhatt**  
