#  Flight Delay Prediction

##  Project Overview

This project aims to predict whether a flight will be delayed by more than 15 minutes using historical flight data and Machine Learning classification models.

The project covers the complete Machine Learning workflow, including data cleaning, exploratory data analysis (EDA), feature engineering, preprocessing, model training, and model evaluation.

---

##  Dataset

- Source: Flight performance dataset
- Size: 100,000 flight records
- Target Variable:
  - **Delayed = 1** → Arrival delay > 15 minutes
  - **Delayed = 0** → Otherwise

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Joblib

---

## ⚙️ Machine Learning Workflow

- Data Cleaning
- Missing Value Handling
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Feature Encoding
- Train/Test Split
- Machine Learning Pipelines
- Model Training
- Model Evaluation
- Model Comparison
- Model Saving

---

## 🤖 Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- XGBoost + SMOTE

---

## 📊 Model Performance

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Logistic Regression | 0.594 | 0.248 | **0.590** | **0.349** |
| Decision Tree | 0.723 | 0.234 | 0.220 | 0.227 |
| Random Forest | 0.808 | 0.343 | 0.044 | 0.078 |
| XGBoost | 0.814 | 0.426 | 0.015 | 0.030 |
| XGBoost + SMOTE | **0.815** | **0.553** | 0.006 | 0.012 |

---

## 📈 Key Insights

- The dataset is imbalanced.
- Accuracy alone is not sufficient for evaluating model performance.
- Logistic Regression achieved the highest Recall and F1-score for detecting delayed flights.
- XGBoost achieved the highest Accuracy but struggled to identify delayed flights.

---


## 💾 Saved Model

The trained Logistic Regression Pipeline was saved using Joblib.

```
flight_delay_model.pkl
```
