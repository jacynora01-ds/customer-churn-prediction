# Customer Churn Prediction and Analysis

## Project Overview
This project uses machine learning to analyse customer churn patterns,
identify factors associated with subscription cancellations, and predict
customer churn.

## Objectives
- Calculate customer churn rate.
- Estimate Customer Lifetime Value (CLV).
- Estimate monthly revenue loss.
- Analyse churn across contract types, payment methods, and subscriptions.
- Build and compare machine learning classification models.

## Dataset
- Total records: 800
- Input features: 11
- Target variable: Churn

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab

## Machine Learning Models
1. Logistic Regression
2. Random Forest Classifier

## Model Performance

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 63.75% | 59.38% |
| Precision | 57.63% | 51.52% |
| Recall | 50.75% | 50.75% |
| F1-Score | 53.97% | 51.13% |

## Key Findings
- Overall churn rate: 41.75%.
- Estimated monthly revenue loss: ₹250,382.29.
- Average customer lifetime value: ₹28,017.59.
- Month-to-month contracts have the highest churn rate.

## Project Files
- Customer_Churn_Prediction.ipynb
- Customer_Churn_Analysis_Report.pdf
- churn_predictions.csv
- customer_churn_model_v2.csv
- report.md
- requirements.txt

## Conclusion
Logistic Regression performed better than Random Forest on the
reported test-set accuracy and F1-score. The analysis highlights
customer segments that may benefit from targeted retention strategies.
