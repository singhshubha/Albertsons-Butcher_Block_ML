# 🧠 Store Profitability ML Project (Meat & Seafood Departments)

This project applies machine learning and data analysis techniques to classify store performance, predict shrink, and extract actionable insights from operational data in the Meat and Seafood departments. The objective is to help identify improvement opportunities, reduce shrink losses, and optimize labor and markdown strategy.

---

## 📌 Project Highlights

- 🔍 Performance categorization using fixed business rules (High, Medium, Unprofitable)
- 📉 Shrink prediction using gradient boosted trees (XGBoost)
- 🧠 Store profitability classification using XGBoost
- 📊 Visual EDA: boxplots, scatter plots, and distributions
- 🧩 Segmentation by revenue, shrink control, and efficiency
- 📈 Feature importance analysis for model interpretability

---

## 🧠 ML Models Overview

### 1. **Shrink Prediction (Regression)**
- **Goal**: Predict weekly shrink in the Meat department
- **Model**: XGBoost (tuned via cross-validation)
- **Features**: Sales, Markdown, Labor Hours, etc.
- **Metrics**: RMSE, MAE, R²

### 2. **Performance Classification**
- **Goal**: Classify store performance as `High`, `Medium`, or `Unprofitable`
- **Model**: XGBoost (classification mode)
- **Features**: Sales, Shrink %, Markdown, Labor Hours, etc.
- **Metrics**: Accuracy, Kappa, Confusion Matrix

---

## 📊 Exploratory Analysis

- Distribution of stores by performance tier
- Boxplots of Sales, Shrink %, and Labor by tier
- Scatterplots of Sales vs Shrink and Sales/Labor efficiency
- Department


##  This is currently an ongoing project
- Updates as I go
