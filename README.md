# IEEE-CIS-Fraud-Detection
Fraud Prevention System using ML

# Overview
The IEEE-CIS Fraud Detection competition invites participants to develop machine learning models to predict the probability that an online transaction is fraudulent. The dataset, provided by Vesta Corporation, consists of real-world e-commerce transactions and includes various features related to transactions and identity information.

# Dataset Description
The data is split into two files: identity and transaction, which are joined by the TransactionID. Some transactions may not have corresponding identity information.

# Files
train_transaction.csv: Contains transaction data for the training set.
train_identity.csv: Contains identity information for the training set.
test_transaction.csv: Contains transaction data for the test set. You need to predict the isFraud value for these observations.
test_identity.csv: Contains identity information for the test set.
sample_submission.csv: A sample submission file in the correct format.
# Features
Categorical Features - Transaction:

ProductCD
card1 to card6
addr1, addr2
P_emaildomain
R_emaildomain
M1 to M9
Categorical Features - Identity:

DeviceType
DeviceInfo
id_12 to id_38
Other Features:

TransactionDT: A timedelta from a given reference datetime (not an actual timestamp).
Evaluation
Submissions are evaluated based on the Area Under the ROC Curve (AUC) between the predicted probabilities and the observed isFraud values.

Submission Format
Your submission file should be a CSV with the following format:

csv
Copy code
TransactionID,isFraud
3663549,0.5
3663550,0.5
3663551,0.5
...
Each TransactionID in the test set should have a corresponding predicted probability for the isFraud variable.

# Citation
Addison Howard, Bernadette Bouchon-Meunier, IEEE CIS, inversion, John Lei, Lynn@Vesta, Marcus2010, Prof. Hussein Abbass. (2019). IEEE-CIS Fraud Detection. Kaggle. Link to competition

