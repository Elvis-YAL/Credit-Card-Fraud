# Credit Card Fraud : Project Overview
* Create a model to predict credit card fraud that enable users to more vigilant against suspicious fraud indicators.  
* Optimized models using Catboost, SMOTE, AutoEncoder to achieve the final desired outcomes.


The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

# What I do

I use Traditional Machine Learning and Catboost to predict credit card fraud. 
Also, I try some unsupervised learning such as autoencoder and evaluate with the label of fraud data.

Here's the picture of Autoencoder result. I plot normal and fraud data with two dimensional, and it's envident that the data has been segregated into categories of normal and fraud data.

![image](https://github.com/Elvis-YAL/Credit-Card-Fraud/assets/40426433/1fdca1e4-a8e3-4956-a323-3f485b9c52bc)
