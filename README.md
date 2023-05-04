# Customer-Lifetime-Value-using-ML

## Introduction
Customer lifetime value (CLV) is one of the key stats likely to be tracked as part of a customer experience program. CLV is a measurement of how valuable a customer is to your company with an unlimited time span as opposed to just the first purchase. This metric helps you understand a reasonable cost per acquisition. CLV is the total worth to a business of a customer over the whole period of their relationship. It’s an important metric as it costs less to keep existing customers than it does to acquire new ones, so increasing the value of your existing customers is a great way to drive growth.

## Data
We have a set of transactional data.
We have 3 years of transactions between Apr '18 and Mar '21.
There is a cohort of 50K customers that purchased for first time the first 3 months, Apr '18 to June '18.

We Frame the problem defining the prediction period. In our example this period will be 6 months aka 26 weeks:
Split the dataset into train and test sample
What will the customers spend the next 6 months, 26 weeks (Regression)
What is a probability of a customer to make a purchase the next 26 weeks (Clasification)

## Feature Engineering
Below we implement functions to compute the features we need. We are performing RFM analysis and so we need to compute the Recency, Frequency and Average Monetary Value for each customer.
Keep in mind, we can add additional features too, but they would need to be aggregated across each customer.

### RFM (Recency-Frequency-Monetary Value)
Recency: How recent is a buyer, when was the last purchase before the end of training period
Frequency: How many purchases a customer made during the training period
Monetary: Mean and Sum of spend during the training period

## Machine Learning Process using XGBoost
XGBoost is a machine learning algorithm that uses an ensemble of decision trees and gradient boosting to make predictions. It is widely used in data science and has won several machine learning competitions.
It is a versatile algorithm that can be used for both classification and regression problems. It can handle different types of data and can be customized for specific needs.

## Conclusions
