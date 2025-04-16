# 🔍 Demand Forecasting with Machine Learning

## 🚀 Overview

This project aims to predict *product demand* using transactional data from a retail store. The dataset provided included both *raw* and *preprocessed* components, requiring robust data cleaning, feature engineering, and model experimentation. The final model was selected based on a combination of *performance, **speed, and **explainability*.

---

## 📁 Dataset Description

- Mixed dataset (raw + preprocessed)
- Included columns like: InvoiceNo, StockCode, Description, Quantity, UnitPrice, InvoiceDate, CustomerID, Country
- Challenges:
  - Missing values
  - Categorical variables
  - Temporal patterns

---

## 🧹 Data Preprocessing

- Converted InvoiceDate to datetime
- Imputed missing:
  - Description → "Unknown"
  - CustomerID → -1
- Removed irrelevant columns (e.g. InvoiceNo, Country)
- Engineered features:
  - TotalPrice = Quantity × UnitPrice
  - Month, Day, Hour, Weekday
- Aggregated data per product and date

---

## 🧠 Models Tried

| Model         | RMSE     | R² Score | Notes                             |
|---------------|----------|----------|-----------------------------------|
| XGBoost       | ~68.5    | ~0.31    | Slow, slightly lower performance  |
| Random Forest | *67.31| **0.33* | Chosen model – faster & explainable   |

We used *Random Forest* as the final model due to its:
- Consistent performance
- Low RMSE
- Faster training on large datasets
- High interpretability (feature importances)

---

## 🧪 Evaluation Metrics

- *RMSE*: 67.31
- *R² Score*: 0.33
- Feature Importance Plots
- Actual vs. Predicted Quantity Scatter Plot

*Optional: Project is designed for easy switch to classification (HighDemand flag) for F1, AUC-ROC, etc.*

---

## 📊 Model Explainability

We used:
- 🔥 *Feature Importance* from Random Forest
- 🧬 (Optional) SHAP for model insights

---

## 🏆 Why This Project Stands Out

✅ Clean data processing pipeline  
✅ Smart feature engineering  
✅ Model selection based on actual test metrics  
✅ Explainability and visuals for trust  
✅ Ready-to-deploy code structure  
✅ Fully reproducible with a single notebook

---

## 🛠 Tech Stack

- *Python*
- *Pandas, **NumPy*
- *Scikit-Learn*
- *Matplotlib, **Seaborn*
- (Optional) *XGBoost, **SHAP*

---

## 📌 Judging Criteria Coverage

| Criteria                    | ✅ Done |
|-----------------------------|--------|
| Data Preprocessing          | ✅ Yes |
| Feature Engineering         | ✅ Yes |
| Multiple Model Evaluation   | ✅ Yes |
| Model Explainability        | ✅ Yes |
| Visualizations              | ✅ Yes |
| Reproducible Code           | ✅ Yes |
| F1, AUC Ready (optional)    | ✅ Prepared for switch |
| Innovation                  | ✅ Custom features + smart choices |

---

## 🔗 Submission

- *Source Code*: [GitHub Repo Link](https://github.com/your-repo-here)
- *Final Notebook*: final_model.ipynb
- *Presentation*: [Available separately]

---

## 📬 Contact

For any questions or issues, open an issue or contact your-ayushkrsna01@gmail.com.

---
