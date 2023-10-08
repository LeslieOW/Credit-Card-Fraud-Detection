# Credit-Card-Fraud-Detection
# Context
Credit card companies handle a vast number of transactions every second. However, some transactions may not be initiated by the cardholder but rather by individuals who illegally possess the cardholder's information. These individuals can initiate fraudulent transactions, causing the rightful cardholders to be charged for items they did not purchase. Therefore, it is essential for credit card companies to identify and prevent these fraudulent transactions.

Maintaining minimal to no instances of fraud not only enhances the trust of customers who prefer using cards for their purchases but also attracts new customers to the business. This, in turn, upholds the company's reputation and contributes to revenue growth by reducing customer attrition and drawing in more customers.

# Data Content
The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Due to confidentiality issues, original features and more background information about the data cannot not be provided. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, the recommended measure of accuracy is the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

# Problem Statement
The challenge is to build a machine learning model that accurately identifies fraud while minimizing false positives.
