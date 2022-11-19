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

The RandomOverSampler has an accuracy score of 64%, total precision score of 99% and total recall score of 60%

![Screenshot 2022-11-13 133614](https://user-images.githubusercontent.com/108438270/201543437-14ffcf10-6d66-47dc-ae63-5102cd388d84.png)


### SMOTE model

The results are pretty similar to the previous model.
The balanced accuracy score is 64%.
The SMOTE Oversampling has a total precision score of 99% and total recall score of 60%

![Screenshot 2022-11-13 133829](https://user-images.githubusercontent.com/108438270/201543566-1e761485-79ab-4005-a442-c93bce7da849.png)




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

