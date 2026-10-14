# customer-churn-project-plan
Project plan and strategy for an E-Commerce Customer Churn Prediction model
# E-Commerce Customer Churn Prediction Model

![Status](https://img.shields.io/badge/Status-Week%201%20Completed-success)
![Role](https://img.shields.io/badge/Role-Data%20Science%20Project%20Coordinator%20Intern-blue)
![Organization](https://img.shields.io/badge/Organization-YuvaIntern%20%7C%20Henry%20Harvin-orange)
![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)

## 📌 Project Overview
Customer retention is one of the most critical growth pillars for modern e-commerce platforms. Acquiring a new customer costs 5x to 7x more than retaining an existing one. This project develops an end-to-end **Machine Learning Customer Churn Prediction Pipeline** to identify high-risk customers before they leave the platform and uncover the key behavioral, transactional, and logistical drivers behind customer attrition.

### 👤 Intern & Project Metadata
* **Intern Name:** Vedant
* **Designation:** Data Science Project Coordinator Intern
* **Organization:** YuvaIntern (in collaboration with Henry Harvin)
* **Current Milestone:** Week 1 — Project Initiation, Scope Definition, Risk Governance & Repository Architecture

---

## 🎯 Project Objectives
1. **Predictive Accuracy & High Recall:** Train and optimize supervised classification models (`Logistic Regression`, `Random Forest`, `XGBoost`) to detect churning customers with strong **Recall**, **F1-Score**, and **ROC-AUC**.
2. **Actionable Business Insights:** Quantify key churn drivers across customer tenure, satisfaction scores, complaint history, app engagement, and delivery distance.
3. **Structured Project Coordination:** Maintain a reproducible, modular codebase with weekly milestone tracking, risk mitigation, and comprehensive documentation.

---

## 🗂️ Repository Architecture
```text
ecommerce-customer-churn-prediction/
│
├── data/
│   ├── raw/                        # Original immutable dataset files
│   └── processed/                  # Cleaned and feature-engineered datasets
│
├── docs/
│   └── Vedant_Data_Science_Week1_Project_Plan.docx   # Week 1 Project Plan Deliverable
│
├── notebooks/
│   ├── 01_exploratory_data_analysis.ipynb
│   ├── 02_feature_engineering.ipynb
│   └── 03_model_training_and_evaluation.ipynb
│
├── src/
│   ├── __init__.py
│   ├── data_preprocessing.py       # Missing value imputation & outlier treatment
│   ├── feature_engineering.py      # Encoding, scaling & SMOTE pipelines
│   └── evaluate_model.py           # ROC-AUC, Precision-Recall & confusion matrices
│
├── reports/
│   └── figures/                    # Generated visual plots and evaluation charts
│
├── .gitignore
├── requirements.txt
└── README.md
```

---

## 📅 5-Week Development Roadmap (WBS)

| Week | Milestone Phase | Key Activities & Deliverables | Status |
| :--- | :--- | :--- | :--- |
| **Week 1** | **Project Planning & Setup** | Define project scope, dataset schema, risk matrix, WBS timeline, and initialize GitHub repository. | ✅ Completed |
| **Week 2** | **Data Cleaning & EDA** | Audit dataset quality, impute missing values, treat outliers, and conduct univariate/bivariate visual analysis. | ⏳ Upcoming |
| **Week 3** | **Feature Engineering & Baseline** | Encode categorical features, scale numerical variables, apply SMOTE for class imbalance, and train baseline models. | 📅 Planned |
| **Week 4** | **Model Optimization & Evaluation** | Hyperparameter tuning (`Random Forest`, `XGBoost`), threshold optimization, and SHAP feature importance analysis. | 📅 Planned |
| **Week 5** | **Final Documentation & Handover** | Compile executive business recommendations, finalize codebase documentation, and submit final presentation. | 📅 Planned |

---

## ⚠️ Risk Management Summary
* **RSK-01 (Class Imbalance):** Mitigated via `SMOTE` (Synthetic Minority Over-sampling Technique) within stratified training folds and evaluated using Precision-Recall AUC rather than raw accuracy.
* **RSK-02 (Missing Behavioral Values):** Mitigated via automated median/KNN imputation pipelines after analyzing missingness patterns in Week 2.
* **RSK-03 (Model Overfitting):** Mitigated via 5-fold Stratified Cross-Validation, regularization constraints, and early stopping rounds.

---

## 🛠️ Tech Stack & Dependencies
* **Language:** Python 3.10+
* **Data Manipulation:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`, `plotly`
* **Machine Learning:** `scikit-learn`, `xgboost`, `imbalanced-learn`, `shap`

## 🚀 Getting Started
```bash
# Clone the repository
git clone [https://github.com/your-username/ecommerce-customer-churn-prediction.git](https://github.com/your-username/ecommerce-customer-churn-prediction.git)

# Navigate into the directory
cd ecommerce-customer-churn-prediction

# Install dependencies
pip install -r requirements.txt
```
