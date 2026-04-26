# 📊 Customer Credit Risk Assessment Model

## Project Overview
This project focuses on predicting customer credit risk using engineered proxy labels derived from financial behaviour and credit characteristics.

---

## Business Problem
The original default variable lacked predictive signal, requiring the development of a new proxy target to simulate real-world credit risk.

---

## Objectives
- Reconstruct a meaningful target variable
- Build predictive models for credit risk classification
- Evaluate trade-offs between precision and recall

---

## Dataset Description
The dataset includes customer demographic and financial attributes such as age, income, loan amounts, and credit scores. Additional behavioral features were engineered to capture financial risk patterns.

---

## Methodology

### Data Preparation
- Cleaned and standardized dataset
- Engineered financial ratios and aggregated customer behavior

### Target Engineering
- Created composite risk score (all_scores_included)
- Introduced stochastic scoring within credit bands
- Derived binary classification label from thresholding

### Modeling
- Logistic Regression
- Random Forest
- XGBoost

### Evaluation
- Precision
- Recall
- F1 Score
- Accuracy

---

## Model Performance

| Model | Recall | Precision | F1 Score | Accuracy |
|------|--------|----------|----------|----------|
| Logistic Regression | 0.740 | 0.681 | 0.709 | 0.697 |
| Random Forest | 0.773 | 0.739 | 0.756 | 0.750 |
| XGBoost | 0.771 | 0.750 | 0.760 | 0.757 |

---

## Insights
- Target quality significantly impacts model performance
- Feature-engineered targets can simulate real-world scenarios
- Tree-based models perform better for nonlinear financial patterns

---

## Challenges
- Target leakage and label reliability
- Balancing performance with interpretability

---

## Conclusion
XGBoost achieved the best balance between precision and recall, making it the most suitable model for identifying high-risk customers.

---

## Project Structure

├── data/
├── notebooks/
├── models/
├── dashboard/
└── README.md

---

## Future Work
- Incorporate real-world default data
- Implement cost-sensitive learning
- Deploy model via API

---

## Dashboard Preview
(Add screenshots here)
