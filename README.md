# Customer-Churn-Prediction-Retention-Strategy
Customer churn is a major revenue challenge for telecom companies
. This project builds an end‑to‑end machine learning solution to predict customer churn and provide actionable business insights that help reduce churn through targeted retention strategies.

Role simulated: Data Scientist
Industry: Telecommunications

🎯 Business Objective

Predict whether a customer will churn (Yes/No)

Identify the key drivers of churn

Support business teams with data‑driven retention actions

Business KPI: Reduce churn by 10–15% by proactively targeting high‑risk customers.

📊 Dataset

Source: Telco Customer Churn (Kaggle)

Size: ~7,000 customers

Target variable: Churn

Features include:

Customer demographics

Contract & subscription details

Billing & payment information

🧹 Data Cleaning

Converted TotalCharges to numeric

Handled missing values (new customers)

Removed non‑informative ID column

Encoded categorical variables (Label Encoding + One‑Hot Encoding)

Scaled numerical features for linear models

🔧 Feature Engineering

Key engineered features:

Customer_Lifetime: tenure in months

AvgMonthlySpend: TotalCharges / tenure

Contract_Risk: risk score based on contract type

These features significantly improved model performance and interpretability.

🧠 Modeling

Models trained and compared:

Logistic Regression (baseline & explainability)

Random Forest (non‑linear patterns)

XGBoost / Gradient Boosting (best performance)

Train/test split: 80/20 with stratification on churn.

📈 Evaluation Metrics

ROC‑AUC (ranking churn risk)

Precision & Recall (business‑critical)

Confusion Matrix

Best model: Gradient Boosting / XGBoost with highest ROC‑AUC and recall on churners.

🔍 Model Explainability

Feature importance analysis

SHAP values to explain individual predictions

Top churn drivers:

Contract type (month‑to‑month)

Customer tenure

Monthly charges

Tech support & online security

💡 Business Insights & Recommendations

Month‑to‑month customers churn ~3× more than long‑term contracts

High monthly charges + no tech support = high churn risk

First 3–6 months are critical for retention

Recommended actions:

Offer contract upgrade discounts to high‑risk users

Bundle tech support for new customers

Launch early‑engagement retention campaigns

🛠️ Tools & Technologies

Python, Pandas, NumPy

Scikit‑learn

XGBoost / Gradient Boosting

SHAP

Matplotlib / Seaborn

📌 Results

This project demonstrates how machine learning can be used not only to predict churn, but also to drive real business decisions and measurable impact.

📬 Contact

For questions or collaboration, feel free to connect via LinkedIn or GitHub.
