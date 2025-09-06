# Bank Customer Churn Prediction

## Project Overview
Customer churn is a major challenge in the banking industry, as retaining existing customers is often more cost-effective than acquiring new ones.  
This project analyzes customer data from a retail bank to predict churn and identify key factors influencing customer attrition. The notebook demonstrates a complete data science pipeline: **Exploratory Data Analysis (EDA), feature engineering, model building, and evaluation.**

---

## Objectives
- Perform **EDA** to understand customer demographics and behavior.  
- Engineer features such as tenure categories, activity levels, and balance groups.  
- Handle class imbalance and prepare data for machine learning.  
- Build and evaluate classification models (Logistic Regression, Random Forest, XGBoost, etc.).  
- Identify the most important **drivers of customer churn**.  

---

## Dataset
- **Source:** Publicly available Bank Customer Churn dataset (Kaggle/UCI).  
- **Rows:** ~10,000 customers  
- **Columns:** 12 features (demographic + financial attributes)  
- **Target Variable:**  
  - `0` → Customer stayed  
  - `1` → Customer churned  

**Key Features:**  
- Geography, Gender, Age, Tenure  
- Balance, Credit Score, Number of Products  
- Has Credit Card, Is Active Member  
- Estimated Salary  

---

## Tools & Libraries
- **Python**
- **Pandas, NumPy** → Data preprocessing and manipulation  
- **Matplotlib, Seaborn** → Visualizations  
- **Scikit-learn** → Model building and evaluation  
- **Imbalanced-learn** → Handling class imbalance  
- **XGBoost** → Gradient boosting classification  

---

## Workflow
1. **Data Exploration**  
   - Checked shape, missing values, summary statistics.  
   - Visualized churn distribution (imbalanced dataset).  

2. **Univariate & Bivariate Analysis**  
   - Distribution of age, balance, credit score.  
   - Churn rates across geography, gender, and activity status.  
   - Heatmaps for correlations.  

3. **Feature Engineering & Preprocessing**  
   - Encoded categorical variables (Gender, Geography).  
   - Created tenure and balance categories.  
   - Applied scaling for numerical features.  
   - Addressed imbalance using **SMOTE/oversampling**.  

4. **Model Development**  
   - Logistic Regression  
   - Random Forest  
   - XGBoost  
   - Hyperparameter tuning with GridSearchCV  

5. **Model Evaluation**  
   - Compared models using Accuracy, Precision, Recall, F1-Score, and ROC-AUC.  
   - Plotted confusion matrices and ROC curves.  

---

## Results
| Model               | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---------------------|----------|-----------|--------|----------|---------|
| Logistic Regression |          |           |        |          |         |
| Random Forest       |          |           |        |          |         |
| XGBoost             |          |           |        |          |         |

*(Fill in with results from your notebook.)*  

---

## Key Insights
- **Strong Predictors:** Customer activity, balance, and age.  
- Customers with **low tenure and low activity** are more likely to churn.  
- **Geographic differences** in churn rates were observed.  
- Class imbalance affects performance, highlighting the importance of recall-focused evaluation.  

---

## Future Work
- Deploy the model using Flask or Streamlit.  
- Build a real-time churn prediction dashboard.  
- Use explainability techniques (e.g., SHAP) for better model interpretation.  

---

## How to Run
1. Clone this repository:  
   ```bash
   git clone https://github.com/thvarsha00/Bank-Customer-Churn-Prediction.git
   cd Bank-Customer-Churn-Prediction

