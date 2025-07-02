# 🧠 Store Profitability ML Project (Meat & Seafood Departments)

This project applies machine learning and data analysis techniques to classify store performance, predict shrink, and extract actionable insights from operational data in the Meat and Seafood departments. The objective is to help identify improvement opportunities, reduce shrink losses, optimize labor and markdown strategy, and provide **data-driven butcher block optimization recommendations**.

---

## 📌 Project Highlights

- 🔍 Performance categorization using fixed business rules (High, Medium, Unprofitable)
- 📉 Shrink prediction using gradient boosted trees (XGBoost)
- 🧠 Store profitability classification using XGBoost
- 📊 Visual EDA: boxplots, scatter plots, and distributions
- 🧩 Segmentation by revenue, shrink control, and efficiency
- 📈 Feature importance analysis for model interpretability
- **🔧 Butcher block optimization with ROI analysis and payback calculations**
- **💰 Shrinkage impact modeling for equipment modifications**

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

### 3. **Butcher Block Optimization (Business Logic)**
- **Goal**: Recommend optimal butcher block configurations to reduce shrink and improve ROI
- **Approach**: Performance-based downsizing with 4ft block constraints
- **Features**: Sales performance, shrink rates, block efficiency metrics
- **Outputs**: Setup costs, payback periods, annual ROI, shrinkage impact

---

## 📊 Exploratory Analysis

- Distribution of stores by performance tier
- Boxplots of Sales, Shrink %, and Labor by tier
- Scatterplots of Sales vs Shrink and Sales/Labor efficiency
- **Block length vs sales efficiency analysis**
- **Setup cost vs weekly savings visualization**
- **Payback period distribution by priority tier**

---

## 🔧 Butcher Block Optimization Features

### **Operational Constraints**
- **4ft block increments only** - realistic equipment modifications
- **Minimum sizes enforced**: Meat (4ft), Seafood (8ft)
- **Performance-based recommendations**: Only suggest changes for underperforming stores

### **Financial Analysis**
- **Setup cost calculations**: Equipment + installation costs
- **Payback period analysis**: Weeks to recoup investment
- **Annual ROI calculations**: Based on shrinkage reduction savings
- **Priority scoring**: HIGH/MEDIUM/LOW based on payback speed and savings

### **Shrinkage Impact Modeling**
- **Quantified shrink reduction**: 0.2% improvement per 4ft meat block removal
- **Weekly dollar savings**: Direct impact on store profitability  
- **Before/after shrink percentages**: Clear improvement metrics
- **"NO MODIFICATIONS" logic**: Only recommend when financially justified

### **Recommendation Outputs**
- Specific block removal suggestions (e.g., "REMOVE 4 feet (1 block)")
- Detailed cost-benefit analysis for each store
- Payback timelines and ROI projections
- Shrinkage impact summaries

---

## 📈 Business Impact & Actionable Insights

- **Store segmentation** for targeted improvement strategies
- **Predictive shrink modeling** for proactive inventory management
- **Performance classification** for resource allocation decisions
- **Equipment optimization recommendations** with clear financial justification
- **ROI-driven decision making** for capital expenditure planning

---

## 🛠️ Tech Stack

- **Language**: R
- **ML Framework**: tidymodels, XGBoost
- **Visualization**: ggplot2, patchwork, gridExtra
- **Data Processing**: dplyr, tidyverse
- **Reporting**: knitr, scales

---

## 📁 Project Structure

```
├── data/
│   └── sample_data.csv
├── scripts/
│   ├── data_preprocessing.R
│   ├── ml_models.R
│   └── butcher_block_optimization.R
├── visualizations/
│   ├── performance_analysis.png
│   └── roi_analysis.png
├── reports/
│   └── store_profitability_analysis.html
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
```r
# Required R packages
install.packages(c(
  "tidyverse", "tidymodels", "xgboost", 
  "vip", "patchwork", "knitr", "scales"
))
```

### Usage
1. Clone the repository
2. Load your data into `data/sample_data.csv`
3. Run the analysis scripts in order:
   - Data preprocessing
   - ML model training
   - Butcher block optimization
4. Generate reports and visualizations

---

## 🎯 Current Status & Future Enhancements

### **Completed Components**
✅ ML models for shrink prediction and performance classification  
✅ Comprehensive EDA and store segmentation analysis  
✅ Butcher block optimization with financial modeling  
✅ ROI analysis and payback calculations  
✅ Shrinkage impact quantification  

### **In Progress**
🔄 Model deployment pipeline  
🔄 Interactive dashboard development  
🔄 Automated recommendation reporting  

### **Future Enhancements**
🔮 Real-time shrink monitoring integration  
🔮 Seasonal demand forecasting  
🔮 Multi-department optimization expansion  
🔮 A/B testing framework for recommendation validation  

---

## 📊 Sample Results

| Store ID | Recommendation | Setup Cost | Payback (Weeks) | Annual ROI |
|----------|----------------|------------|-----------------|------------|
| 12345 | Remove 4ft meat block | $1,100 | 24 | 135% |
| 67890 | Remove 8ft seafood block | $2,100 | 18 | 187% |

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/enhancement`)
3. Commit changes (`git commit -am 'Add enhancement'`)
4. Push to branch (`git push origin feature/enhancement`)
5. Create Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📧 Contact

**Shubha S Singh**  
- Email: [your.email@example.com]
- LinkedIn: [your-linkedin-profile]
- GitHub: [your-github-username]

---

*This is an ongoing project with continuous updates and improvements based on business feedback and performance validation.*
