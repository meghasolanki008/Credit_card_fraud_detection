# Credit Card Fraud Detection

Dataset of this project is available in :
[Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

# Problem Statement
A credit card is one of the most used financial products to make online purchases and payments. Though the Credit cards can be a convenient way to manage your finances, they can also be risky. Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash.

It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

We have to build a classification model to predict whether a transaction is fraudulent or not.

# Contents

### 1.Dataset overview
The dataset contains 2,84,807 records and 31 features.

The features names are 'Time', 'Amount','Class','V1', 'V2', 'V3', 'V4', 'V5', 'V6', 'V7', 'V8', 'V9', 'V10','V11', 'V12', 'V13', 'V14', 'V15', 'V16', 'V17', 'V18', 'V19', 'V20','V21', 'V22', 'V23', 'V24', 'V25', 'V26', 'V27', 'V28'

Due to confidentiality issues, we cannot have the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'.

'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset.

The feature 'Amount' is the transaction Amount.

Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

### 2.Data Cleaning and Data Preprocessing
* Null values detection
* Missing values detection
* Duplicated values detection
* Standardisation of dataset
* Imbalanced Data detection
* Handled Imbalanced data using SMOTE

### 3. Train-test split
* Featue Engineering
* Feature extraction
* Feature Importance


### 4. Modeling
* Logistic Regression Classifier
* Decision Tree Classifier
* Random Forest Classifier

### 5. Evaluation

* ROC AUC Score
* ROC Curve
* Confusion Matrix
* Classification report

### 6. Conclusion
Decision Tree and Random Forest Classifier gives a better accuracy score of 99.94%
      

      
      
