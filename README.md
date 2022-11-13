# Credit_Risk_Analysis

## Overview

Predicting Credit Risk. 
The goal of this analysis was to create a supervised machine learning model that would predict credit risk from loan applicants based of the data in the provided csv file. Information factors included loan size, interest rate, borrower income, debt to income ratio, number of accounts they have, derogatory marks, and total debt.


## Resources

- Data Source: LoanStats_2019Q1.csv
- Software: Python 3.7.9 
Anaconda Navigator 1.9.12
Conda 4.8.4
Jupyter Notebook 6.0.3


## Results

### RandomOverSampler model

The balanced accuracy score is 65%.
The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

### SMOTE model

The results are pretty similar to the previous model.
The balanced accuracy score is 64%.
The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.


### ClusterCentroids model

Here the balanced accuracy score is down to about 52%.
The high_risk precision is still 1% only with 63% sensitivity which makes a F1 of 1%.
Due to the high number of false positives, the low_risk sensitivity is only 40%.


### 

The balanced accuracy score is about 62%.
The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 57%.


### BalancedRandomForestClassifier model

The balanced accuracy score improved to about 79%.
The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.


### EasyEnsembleClassifier model

The balanced accuracy score is high to about 93%.
The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.


## Summary

The Ensemble models brought a lot more improvment specially on the sensitivity of the high risk credits.
The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit. 
All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high.

