# Classification Modeling: analyzing customer churn within Telco

## About the Project
Reducing churn is one of the biggest challenges facing subscripition based services. The costs of retaining customers far outweight the costs of aqcuiring new cusomters. This project will highlight the biggest drivers of customer churn within Telco by builiding a classification model to accurately predict churn.

### Project Overview

The goal of this project is to identify if the internet service type (DSL, Fiber Optic, none) matters when concerning the churn rate of customers. 

Although pricing is important to consumers, the type of service being provided to consumers in the telecommunications space is also important.
This project will analyze isolate and analyze the two types of internet service being provided to Telco's consumers and will determine if
the type of service being provided is related to the churn rate of those customers.

My initial question is "Does the type of internet service being provided to customers affect Telco's revenue?"

## Data Dictionary

**churn**: customer stop using services (yes or no).<br>
**internet_service_type**: none, fiber optic, or DSL (digital subsriber line).<br>


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
