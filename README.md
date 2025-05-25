# 🏦 Bankruptcy Prediction Using Ensemble Learning

## 📘 Project Overview

This project aims to build accurate and interpretable models for **firm-level bankruptcy prediction** using financial ratios. By preprocessing real-world financial data, applying multiple machine learning algorithms, and combining them via ensemble techniques, we aim to deliver a model that can effectively flag financially distressed firms—critical for investors, creditors, and regulators.

## 👥 Team
**Analytics Avengers**  
Project for **MGMT 571 – Final Project**

## 📊 Problem Statement

Predicting bankruptcy is a **high-stakes binary classification problem**, where false negatives (missed bankruptcies) can be especially costly. The financial data includes profitability, liquidity, and liability ratios across various firms. The goal is to build models that balance **accuracy**, **interpretability**, and **generalization**, evaluated primarily by **AUC (Area Under the Curve)**.

## 🧹 Data Preparation

- **Attribute Reduction**: 16 highly correlated financial ratios removed to reduce redundancy and noise.
- **Data Replacement**: Handled missing or invalid values (e.g., net profit, liabilities) using imputation to ensure data integrity.
- **Partitioning**: Split into training, validation, and test sets to avoid overfitting and evaluate generalization.

## 🤖 Models Used

A variety of models were trained and evaluated:

### 🔢 Baseline Models

- **Logistic Regression**: Interpretable and robust for binary classification.
- **Stepwise Logistic Regression (Forward & Backward)**: Helps identify the most significant predictors with reduced complexity.

### 🌲 Gradient Boosting (Default & High Complexity)

- Captures non-linear interactions.
- Two configurations tested to compare overfitting vs. generalization.

### 🧠 Neural Networks

- **High-Performance Neural Network (HP Neural)**: Deep model for capturing subtle dependencies in financial metrics.
- **Custom Neural Network**: Alternative architecture for increased diversity.

### 📈 Polynomial Regression

- Adds polynomial terms to model curved relationships among variables.

## 🧬 Ensemble Models

Three ensembles were built to combine predictions from individual models:

- **Why use ensembles?**
  - Different models capture different data structures.
  - Ensembles reduce both bias and variance.
  - Improves overall prediction accuracy and robustness.

## 🧪 Model Evaluation

- **Metric Used**: Area Under the ROC Curve (AUC)
- **Why AUC?**
  - Robust to class imbalance.
  - Measures the ability to rank firms correctly based on bankruptcy probability.
  - Prioritizes identifying true positives (bankrupt firms).

## 🧠 Key Takeaways

- **Gradient Boosting and Neural Networks** outperformed simpler models due to their ability to model complex patterns.
- **Logistic Regression** provided valuable interpretability.
- **Ensemble Models** delivered the best performance by leveraging model diversity.
- Handling **missing values** and **attribute correlation** was crucial for model reliability.
- Bankruptcy risk is influenced by **non-linear interactions** across profitability, liability, and efficiency metrics.

## 🛠️ Tools & Technologies

- **SAS Enterprise Miner**
- **Python / R (assumed for preprocessing or secondary modeling)**
- **Financial ratio datasets**

## 📌 Conclusion

Our ensemble-based approach to bankruptcy prediction leverages the strengths of both interpretable and complex models. By carefully preprocessing the data and validating across multiple configurations, we build a robust system capable of identifying financially distressed firms before failure—enhancing risk management across financial domains.

---

> _“Bankruptcy prediction isn't just a data science problem—it's a financial early warning system. Our models make that system smarter, faster, and more reliable.”_
