# Classification Modeling: analyzing customer churn within Telco

## About the Project
Reducing churn is one of the biggest challenges facing subscripition based services. The costs of retaining customers far outweight the costs of aqcuiring new cusomters. This project will highlight the biggest drivers of customer churn within Telco by builiding a classification model to accurately predict churn.

### Project Overview

The goal of this project is two-fold. First, identify the main drivers of churn. Second, ask the hypothesis "Do customers who have a higher monthly bill, churn more?"

This project will explore these topics in the form of various classification models, including Logisitic Regression, KNN, Random Forest and Decision Tree. We will split the data into Train, Validate and Test to run our models and evaluate the accuracy of them.

## Data Dictionary
**gender**: female or male.<br>
**senior_citizen**: yes or no.<br>
**partner**: yes or no.<br>
**depedents**: yes or no.<br>
**tenure**: number of months that a customer has subscribed for.<br>
**phone_service**: yes or no.<br> 
**multiple_lines**: yes, no or no phone service.<br> 
**online_security**: yes, no, or no internect service.<br>
**online_backup**: yes, no, or no internect service.<br>
**tech_support**: yes, no, or no internect service.<br>
**streaming_tv**: yes, no, or no internect service.<br>
**streaming_movies**: yes, no, or no internect service.<br>
**paperless_billing**: yes or no.<br> 
**monthly_charges**: bill for the subscribed services every month (dollars).<br>
**total_charges**: total bill for the subscribed services (dollars).<br>
**churn**: customer stop using services (yes or no).<br>
**contract_type**: month-to-month, one-year or two-year.<br>
**internet_service_type**: none, fiber optic, or DSL (digital subsriber line).<br>
**payment_type**: credit card (automatic), bank transfer (automatic), mailed check or electronic check.<br>


## Project Planning

### acquire.py

obtain the data from the telco_churn database on the Codeup data science database server. 

### Prepare.py

* Identify missing data

* Encode variable as needed

* Drop object columns

* Split data into train/validate/test

### Explore

* Explore target variable:
    * Compute overall churn rate
    * Barplot target variable
    
* Explore `churn`'s interactions with the categorical variables by treating it as a number 
    * Services: internet_service_type


### Modeling and Evaluation

* Build four different algorithms to analyze churn: logistic regression, decision tree, random forest and knn

* Which features are most influential?

* Evaluate on train

* Select top 3 models to evaluate on validate

* Select top model

* Run model on test to verify

### Conclusion

* Summarize findings

* Present key takeaways

* Next steps

### Predictions.csv

* csv file with customer_id, probability of churn, and prediction of churn (1=churn, 0=not_churn)

## How to Reproduce

1. Download data from codeup data science database server (You must be logged in first).
2. Install acquire.py and preapre.py into your working directory.
3. Run the jupyter notebook. 
