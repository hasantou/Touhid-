# PaySim Fraud Detection

End-to-end machine learning project detecting fraud in 6.3 million
synthetic financial transactions using Python.

## Key Findings
- Only CASH_OUT and TRANSFER contain fraud — zero in all other types
- 98.1% of fraud drains the origin account to exactly $0
- Fraud median amount ($441k) is 6x higher than legitimate ($74k)
- Fraud peaks at 4 AM — consistent with automated scripted attacks

## Project Steps
1. Exploratory Data Analysis
2. Feature Engineering
3. Class Imbalance Handling — SMOTE and class weights
4. Model Training — Logistic Regression, Random Forest, Gradient Boosting
5. SHAP Explainability

## Model Results
| Model | Precision | Recall | F1 | AUC-ROC |
|---|---|---|---|---|
| Logistic Regression | 0.0371 | 0.981 | 0.0715 | ~0.9958 |
| Random Forest | ~1.00 | ~0.9976 | ~0.9988 | ~0.9997 |
| Gradient Boosting | ~0.8770 | ~0.9982 | ~0.9337 | ~0.9998 |

## Dataset
PaySim Synthetic Financial Transactions — available on
[Kaggle](https://www.kaggle.com/datasets/ealaxi/paysim1)

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook paysim_fraud_detection.ipynb
```
## Project Report
A full written report covering all five steps of the analysis is available here:
[Download Report](PaySim Fraud Detection Report.pdf)
## Author
Touhid Hasan | MSc Data Science | University of Greenwich
