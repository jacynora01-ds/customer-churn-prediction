# Customer Churn Prediction and Analysis

## 1. Project Overview

This project uses machine learning to analyse customer churn patterns, identify factors associated with subscription cancellations, and predict which customers are likely to churn.

The objective is to help businesses understand customer behaviour, estimate revenue loss, and develop effective customer retention strategies.

## 2. Project Objectives

- Calculate the customer churn rate.
- Estimate Customer Lifetime Value (CLV).
- Calculate estimated monthly revenue loss.
- Identify customer segments with higher churn rates.
- Analyse churn based on contract type.
- Analyse churn based on payment method.
- Analyse churn based on subscription type.
- Build and compare machine learning models.
- Generate customer churn predictions.

## 3. Dataset Information

- Dataset: customer_churn_model_v2.csv
- Total records: 800
- Input features: 11
- Target variable: Churn
- Identifier: CustomerID

CustomerID was excluded from the model training process.

## 4. Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab

## 5. Data Preprocessing

The following preprocessing techniques were used:

- Separated numerical and categorical features.
- Applied MinMaxScaler to numerical features.
- Applied OneHotEncoder to categorical features.
- Divided the dataset into 80% training data and 20% testing data.
- Used stratified sampling to maintain the churn distribution.

## 6. Machine Learning Models

Two classification algorithms were implemented:

1. Logistic Regression
2. Random Forest Classifier

Both models were trained and evaluated using the same training and testing split.

## 7. Model Performance

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 63.75% | 59.38% |
| Precision | 57.63% | 51.52% |
| Recall | 50.75% | 50.75% |
| F1-Score | 53.97% | 51.13% |

Logistic Regression achieved better accuracy and F1-score than Random Forest on the test dataset.

Therefore, Logistic Regression was selected for generating the final customer predictions.

## 8. Business Metrics

| Metric | Result |
|---|---:|
| Total Customers | 800 |
| Churned Customers | 334 |
| Churn Rate | 41.75% |
| Estimated Monthly Revenue Loss | ₹250,382.29 |
| Average Customer Lifetime Value | ₹28,017.59 |
| Average CLV of Churned Customers | ₹27,183.31 |
| Average CLV of Retained Customers | ₹28,615.55 |

## 9. Churn Analysis

### Contract Type

| Contract Type | Retained | Churned |
|---|---:|---:|
| Month-to-Month | 40.97% | 59.03% |
| One Year | 77.21% | 22.79% |
| Two Year | 80.39% | 19.61% |

Month-to-month customers showed the highest churn rate.

### Payment Method

| Payment Method | Retained | Churned |
|---|---:|---:|
| Card | 61.11% | 38.89% |
| Net Banking | 58.79% | 41.21% |
| UPI | 55.92% | 44.08% |
| Wallet | 57.29% | 42.71% |

UPI users showed the highest churn rate among the payment methods.

### Subscription Type

| Subscription Type | Retained | Churned |
|---|---:|---:|
| Basic | 58.99% | 41.01% |
| Pro | 58.04% | 41.96% |
| Standard | 57.68% | 42.32% |

Standard subscription customers showed the highest churn rate, although the differences were small.

## 10. Business Recommendations

1. Encourage month-to-month customers to consider longer-term contracts through renewal discounts.
2. Investigate payment-related difficulties among UPI and Wallet users.
3. Introduce customer loyalty programmes and retention offers.
4. Monitor customers with behavioural patterns associated with higher churn.
5. Improve customer support and investigate recurring service issues.

## 11. Project Files

| File | Description |
|---|---|
| Customer_Churn_Prediction.ipynb | Complete machine learning notebook |
| Customer_Churn_Analysis_Report.pdf | Final project report |
| churn_predictions (1).csv | Customer churn prediction results |
| customer_churn_model_v2.csv | Original dataset |
| report.md | Markdown project report |
| requirements.txt | Required Python libraries |

## 12. Conclusion

This project analysed customer churn using an 800-record dataset and implemented two machine learning classification algorithms.

The overall churn rate was 41.75%, with an estimated monthly revenue loss of ₹250,382.29.

Logistic Regression performed better than Random Forest based on test-set accuracy and F1-score.

The analysis identified contract type and payment method as useful areas for further customer retention investigation.

The project demonstrates the application of data preprocessing, exploratory analysis, machine learning, model evaluation, and business interpretation.

---

**Project Category:** Data Analytics / Machine Learning

**Tools:** Python, Google Colab, Scikit-learn
