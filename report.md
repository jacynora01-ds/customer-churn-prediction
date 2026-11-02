
# Customer Churn Prediction and Analysis

## 1. Project Overview

This project analyses customer subscription data to identify churn patterns,
estimate customer lifetime value, and build machine-learning models to predict
customer churn.

## 2. Dataset Overview

- Total customers: 800
- Total features: 11 (excluding CustomerID and Churn)
- Churned customers: 334
- Retained customers: 466

## 3. Business Metrics

- Churn Rate: 41.75%
- Estimated Monthly Revenue Loss: Rs. 250,382.29
- Average Customer Lifetime Value: Rs. 28,017.59
- Average CLV of Churned Customers: Rs. 27,183.31
- Average CLV of Retained Customers: Rs. 28,615.55

## 4. Machine Learning Models

Two classification algorithms were trained:

1. Logistic Regression
2. Random Forest Classifier

An 80:20 train-test split was used.

### Model Performance

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 0.6375 | 0.5938 |
| Precision | 0.5763 | 0.5152 |
| Recall | 0.5075 | 0.5075 |
| F1-Score | 0.5397 | 0.5113 |

Logistic Regression achieved better accuracy and F1-score on the test set.
It was selected for generating the final customer predictions.

## 5. Churn Analysis by Contract Type

Churn              No    Yes
ContractType                
Month-to-Month  40.97  59.03
One Year        77.21  22.79
Two Year        80.39  19.61

Month-to-month customers showed the highest churn rate.

## 6. Churn Analysis by Payment Method

Churn             No    Yes
PaymentMethod              
Card           61.11  38.89
Net Banking    58.79  41.21
UPI            55.92  44.08
Wallet         57.29  42.71

UPI users showed the highest churn rate among the payment methods.

## 7. Churn Analysis by Subscription Type

Churn                No    Yes
SubscriptionType              
Basic             58.99  41.01
Pro               58.04  41.96
Standard          57.68  42.32

Standard subscription customers showed the highest churn rate, although
the differences between subscription types were small.

## 8. Feature Importance

The Random Forest model was used to rank the features by predictive importance.

                         Feature  Importance
            num__TotalChargesINR    0.122876
               num__TenureMonths    0.121853
          num__MonthlyChargesINR    0.119830
                        num__Age    0.110418
               num__LatePayments    0.080698
             num__SupportTickets    0.072810
cat__ContractType_Month-to-Month    0.071972
      cat__ContractType_One Year    0.034520
      cat__ContractType_Two Year    0.028960
               cat__Region_South    0.023446

Feature importance indicates how much the model relied on each feature.
It does not establish causation.

## 9. Business Recommendations

1. Encourage month-to-month customers to consider annual contracts.
2. Investigate payment difficulties among UPI and Wallet users.
3. Monitor customers with behavioural patterns associated with higher churn.
4. Introduce customer retention campaigns and loyalty benefits.
5. Improve customer support and investigate recurring service issues.

## 10. Conclusion

The dataset showed an overall churn rate of 41.75%.
Logistic Regression performed better than Random Forest on the reported
test-set accuracy and F1-score.

The analysis identifies contract type and payment method as useful
areas for further customer-retention investigation.

The predictions and metrics should be interpreted in the context of
the dataset and the limitations of the trained models.
