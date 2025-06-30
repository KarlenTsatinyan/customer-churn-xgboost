
# 📉 Customer Churn Prediction with XGBoost

This project aims to predict customer churn for a telecommunications company using machine learning techniques, including **XGBoost**, **SMOTE** for class balancing, **hyperparameter tuning**, and **feature importance analysis**.

> 💼 Built as part of a data science portfolio to demonstrate skills in EDA, feature engineering, model evaluation, and deployment readiness.

---

## 🗂️ Project Overview

- **Objective**: Predict whether a customer will churn based on their account, demographic, and usage features.
- **Dataset**: [Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Tech Stack**: Python, Pandas, Seaborn, Scikit-learn, XGBoost, SMOTE, Matplotlib

---

## 🧪 Key Features

✅ Feature importance with SHAP and model insights  
✅ SMOTE to handle imbalanced classes  
✅ XGBoost model with hyperparameter tuning  
✅ Evaluation metrics with ROC-AUC, F1, confusion matrix  
✅ Clean, visual EDA  
✅ Ready for deployment (Streamlit/FastAPI-ready)

---

## 📊 Exploratory Data Analysis Highlights

| Feature           | Churn Tendency         |
|-------------------|------------------------|
| `Tenure`          | Short tenure = higher churn |
| `MonthlyCharges`  | Higher charges → more likely to churn |
| `Contract`        | Month-to-month contracts → high churn risk |
| `TotalCharges`    | Low value = newer customers = higher churn |
| `InternetService` | Fiber optic → slightly more churn |

---

## ⚙️ Model Performance

### 🔧 Final Model: XGBoost + SMOTE + Hyperparameter Tuning

| Metric         | Score    |
|----------------|----------|
| Accuracy       | 80%      |
| Precision (1)  | 66%      |
| Recall (1)     | 51%      |
| F1-score (1)   | 0.57     |
| ROC AUC        | 0.71     |

> `Best Params`: `learning_rate=0.1`, `max_depth=3`, `n_estimators=100`, `subsample=0.8`

**Confusion Matrix**:
```
[[936  97]
 [184 190]]
```

---

## 🔍 Business Recommendations

- 🧾 **Incentivize long-term contracts** to reduce churn from short-term users.
- 🤝 **Engage new customers early** — those with short tenure or low TotalCharges are at higher risk.
- 💸 **Re-evaluate pricing or offer bundles** for customers paying high monthly charges.
- 📡 **Improve service for Fiber Optic users**, if correlated with higher churn.

---

## 🚀 Future Improvements

- 🧪 Try additional models (e.g., LightGBM, CatBoost)
- 🧠 Add SHAP-based explainability dashboard
- 🧰 Deploy using Streamlit or FastAPI
- 📈 Monitor churn predictions with real-time dashboards

---

## 📬 Contact

If you'd like to collaborate or have questions, feel free to connect with me via [GitHub](https://github.com/yourusername) or [LinkedIn](https://www.linkedin.com/in/your-link).

---

⭐️ **Star** this repo if you found it useful!  
👀 Feedback, contributions, and suggestions are always welcome.
