# Bank Term Deposit Propensity Modeling

## Overview

This project builds a machine learning model to help a bank improve marketing efficiency.  
The goal is simple: predict which customers are most likely to subscribe to a term deposit before making a call.

Instead of contacting everyone, the bank can prioritize high probability customers and reduce wasted outreach.

---

## The Problem

Bank campaigns typically convert around 12 percent of contacted customers.  
That means most calls do not lead to subscriptions.

This project focuses on improving targeting so marketing efforts are more strategic and cost effective.

---

## Approach

I tested multiple classification models:

Logistic Regression as a baseline  
Decision Tree with hyperparameter tuning  
Random Forest as the final selected model  

A stratified train validation split was used to preserve class imbalance.  
Hyperparameters were tuned using GridSearchCV.  
ROC AUC was used as the primary evaluation metric.

---

## Final Model Performance

Random Forest achieved:

ROC AUC of 0.84  
Precision improved from 12 percent random baseline to 45 percent for top decile targeting  

This means the model significantly improves the bank’s ability to prioritize likely subscribers.

---

## Business Impact

By targeting the top 30 percent of customers ranked by predicted probability:

The bank can capture over 60 percent of total conversions  
Outreach volume can be reduced substantially under optimized threshold selection  

This supports a shift from mass calling to data driven prioritization.

---

## Key Drivers Identified

The most important predictors include:

Account balance  
Age  
Campaign history  
Previous subscription success  
Contact method quality  

These insights support smarter customer segmentation.

---

## Tech Stack

Python  
Pandas  
NumPy  
Scikit learn  
Matplotlib  

---

## Conclusion

This project demonstrates how predictive modeling can support better marketing decisions.  
The final model provides both strong performance and clear business insights that can be used in real campaign planning.
