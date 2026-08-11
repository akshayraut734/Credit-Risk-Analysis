# 💳 Credit Risk Analysis & Default Prediction

An end-to-end Machine Learning and financial risk analytics project designed to evaluate borrower creditworthiness, estimate Probability of Default (PD), and minimize financial losses for lending institutions.

---

## 📌 Project Overview

Credit risk assessment is a fundamental operation in commercial banking and fintech lending. This project builds a predictive modeling pipeline that analyzes applicant financial profiles, credit histories, and loan characteristics to accurately classify high-risk vs. low-risk borrowers, handle class imbalance, and generate actionable credit scoring metrics.

---

## 📊 Key Highlights & Business Impact

* **Probability of Default (PD) Modeling:** Predicts the likelihood of a borrower defaulting on loan obligations.
* **Feature Selection & Scorecard Generation:** Applies Weight of Evidence (WOE) and Information Value (IV) analysis to rank predictive features.
* **Class Imbalance Management:** Implements resampling techniques (SMOTE / Random Oversampling) and class weighting to address the disparity between non-default and default records.
* **Model Validation Metrics:** Evaluates models using ROC-AUC, Gini Coefficient, Kolmogorov-Smirnov (KS) Statistic, Precision-Recall, and Confusion Matrices.

---

## 🛠️ Data Pipeline & Methodology

1. **Exploratory Data Analysis (EDA) & Data Cleaning:**
   * Handled missing value imputation and outlier detection across numerical income and debt-to-income (DTI) metrics.
   * Categorical feature encoding for employment status, home ownership, and loan intent.

2. **Feature Engineering & Selection:**
   * Calculated debt ratios, credit utilization rates, and historical payment performance metrics.
   * Filtered redundant features via correlation heatmaps and Information Value (IV) analysis.

3. **Model Development & Hyperparameter Tuning:**
   * Benchmark Model: **Logistic Regression** (Interpretable baseline for credit scorecards).
   * Tree-Based Models: **Random Forest**, **Decision Trees**, and **XGBoost / LightGBM** for non-linear risk capture.
   * Cross-validation and grid search tuning to optimize ROC-AUC and minimize false negative rates (Type II errors).

---

## 📂 Repository Structure

```text
Credit-Risk-Analysis/
│
├── data/
│   └── credit_risk_dataset.csv        # Historical borrower records and target default indicators
├── notebooks/
│   └── Credit_Risk_Analysis.ipynb     # Data cleaning, EDA, feature selection, and model training
├── README.md                          # Project documentation
└── requirements.txt                    # Project dependencies
