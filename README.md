# 💳 Financial Fraud Detection Using Machine Learning

Financial fraud detection is a critical application of data science and machine learning, aimed at identifying suspicious or anomalous transactions from vast volumes of financial data. This project implements a supervised classification model designed to detect **fraudulent financial transactions**, with a particular focus on handling **imbalanced data**, maximizing **recall**, and minimizing **false negatives**.




## 🧠 Key Machine Learning Concepts

This project demonstrates the practical application of several core concepts in machine learning and data science, including:

- **Data Cleaning & Preprocessing**: Ensuring high-quality inputs by handling missing values, scaling features, and encoding data.
- **Imbalanced Classification**: Using techniques like class weighting to address skewed class distributions.
- **Model Selection & Training**: Employing logistic regression for interpretable results and probabilistic outputs.
- **Evaluation Metrics**: Going beyond accuracy to include ROC AUC, precision-recall curves, F1-score, and confusion matrices to better evaluate models on imbalanced data.
- **Threshold Tuning**: Adjusting the decision threshold to prioritize detection of fraud cases (high recall) while managing false positives.
- **Interpretability**: Understanding model decisions using coefficient analysis and evaluating feature importance.



## 🧾 Dataset Overview

The dataset contains **transaction-level data** for thousands of financial events, with each labeled as either **fraudulent** or **legitimate**. 

### Features:
- `transaction_value`: Amount involved in the transaction.
- `transaction_type`: Category/type of transaction.
- `account_age`: Age of the account in years.
- `location_score`: A proxy for geographic risk.
- `device_trust_score`: Heuristic score of device legitimacy.
- `is_fraud`: Target variable (1 = Fraud, 0 = Legitimate)

> *Note: Column names are anonymized for generalization.*

### Class Distribution:
Fraudulent transactions represent a **very small percentage** of the dataset (~1-2%), which reflects real-world fraud data challenges.

## ⚙️ Tools & Technologies

- **Python 3.8+**
- **pandas** for data manipulation
- **numpy** for numerical operations
- **scikit-learn** for modeling and evaluation
- **matplotlib** and **seaborn** for visualization

## 📈 Performance Summary

Given the importance of **catching fraudulent activity**, high **recall** is prioritized to reduce false negatives. The following metrics were achieved:

- **Accuracy**: 97% (baseline)
- **Precision**: ~0.75
- **Recall**: ~0.88
- **F1-Score**: ~0.81
- **ROC AUC**: ~0.93

> The model shows strong ability to detect fraud while balancing false positives.


## 🔍 Insights & Learnings

- Traditional accuracy is misleading in imbalanced datasets—**recall and precision** are more informative.
- **Logistic regression**, despite its simplicity, performs well with good preprocessing and regularization.
- Feature engineering and interpretability are crucial for real-world adoption in financial institutions.
- Adjusting **thresholds** can help tailor the model to business needs—whether reducing fraud loss or minimizing customer inconvenience.
