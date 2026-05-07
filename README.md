# Customer Churn Prediction

An end-to-end Machine Learning project focused on predicting telecom customer churn and segmenting customers into actionable risk categories using classification models, exploratory data analysis, and business intelligence visualizations.

---

# Project Overview

Customer churn is one of the biggest challenges faced by subscription-based businesses. Predicting which customers are likely to leave helps companies take proactive actions such as offering discounts, improving customer support, and increasing customer engagement.

This project uses the IBM Telco Customer Churn dataset to:

* Predict customer churn using Machine Learning
* Compare multiple classification models
* Segment customers into risk tiers
* Generate business insights and recommendations
* Visualize churn behavior using professional charts and dashboards

This project was completed as part of an **AI & Data Analytics Internship – Week 2 Project**.

---

# Objectives

* Perform Exploratory Data Analysis (EDA)
* Clean and preprocess telecom customer data
* Engineer meaningful features
* Train and compare multiple ML models
* Evaluate models using multiple metrics
* Segment customers into churn risk tiers
* Create professional business visualizations
* Generate actionable business recommendations

---

# Dataset Information

**Dataset:** IBM Telco Customer Churn Dataset

**Source:**
[Kaggle Dataset Link](https://www.kaggle.com/datasets/blastchar/telco-customer-churn?utm_source=chatgpt.com)

### Dataset Features

* Customer demographics
* Contract information
* Internet services
* Payment methods
* Monthly charges
* Total charges
* Customer support services
* Tenure information

### Target Variable

```python
Churn
```

* `Yes` → Customer churned
* `No` → Customer retained

---

# Technologies Used

| Tool / Library   | Purpose                      |
| ---------------- | ---------------------------- |
| Python           | Main Programming Language    |
| Pandas           | Data Analysis & Manipulation |
| NumPy            | Numerical Computation        |
| Scikit-learn     | Machine Learning             |
| Matplotlib       | Data Visualization           |
| Seaborn          | Statistical Visualization    |
| Plotly           | Interactive Visualization    |
| Jupyter Notebook | Development Environment      |

---

# Machine Learning Models

The following classification models were trained and evaluated:

1. Logistic Regression
2. Random Forest Classifier
3. Gradient Boosting Classifier

---

# Evaluation Metrics

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Confusion Matrix
* ROC Curve Comparison

---

# Feature Engineering

Custom engineered features:

```python
ChargesPerMonth = TotalCharges / tenure
```

```python
SeniorWithNoSupport = (SeniorCitizen == 1) & (TechSupport == 'No')
```

---

# Customer Risk Segmentation

Customers were segmented using predicted churn probabilities:

| Risk Tier      | Probability |
| -------------- | ----------- |
| 🔴 High Risk   | ≥ 0.70      |
| 🟡 Medium Risk | 0.40 – 0.69 |
| 🟢 Low Risk    | < 0.40      |

---

# Visualizations Included

* Churn Distribution Chart
* Correlation Heatmap
* Feature Importance Chart
* Confusion Matrices
* ROC Curve Comparison
* Churn Rate by Contract Type
* Tenure Distribution by Churn
* Risk Tier Pie Chart
* Interactive Plotly Scatter Plot

---

# Key Insights

* Month-to-month contract customers had the highest churn probability.
* Customers with high monthly charges were more likely to churn.
* Short-tenure customers showed significantly higher churn risk.
* Lack of technical support services increased churn likelihood.
* Gradient Boosting and Logistic Regression achieved the best ROC-AUC performance.

---

# Business Recommendations

1. Offer discounts and loyalty benefits for long-term contracts.
2. Improve onboarding and customer support for new customers.
3. Create targeted retention campaigns for high-risk customers.
4. Monitor customer churn probability using predictive analytics.

---

# Project Structure

```text
customer-churn-prediction-dashboard/
│
├── Customer_Churn_Analysis.ipynb
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── model_comparison.png
├── summary.docx
├── requirements.txt
│
├── charts/
│   ├── feature_importance.png
│   ├── churn_contract.png
│   ├── tenure_distribution.png
│   └── risk_tier_pie.png
│
└── README.md
```

---

# Installation

Clone the repository:

https://github.com/ankitkumar8558011-alt/customer-churn-prediction.git


Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook:

```bash
jupyter notebook
```

---

# Results

The project successfully built a complete machine learning pipeline for churn prediction and customer risk segmentation. The insights generated from this analysis can help telecom companies improve customer retention strategies and reduce revenue loss caused by churn.

---

# Future Improvements

* Apply XGBoost for better performance
* Use SMOTE to handle class imbalance
* Deploy using Streamlit dashboard
* Add real-time churn prediction
* Improve probability calibration

---

# Author

Ankit kumar 
[AI & Data Analytics Internship Project]

