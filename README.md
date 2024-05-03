# Credit_card_fraud_detection

Credit Card Fraud Detection using Logistic Regression

 * Project - Credit Card Fraud Detection

 * Skills - Logistic regression , Support Vector Machine, K Nearest Neighbours, F1 Score, ROC-AUC Curve, Data Visualisation , Exploratory Data Analysis , Machine Learning
 
 * Tools -  Jupyter Notebooks , Python , Numpy , Pandas , Matplotlib , Seaborn , Sklearn
 
# Dataset

The data was taken from Kaggle site : https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud .

The Columns do not have physical significance directly visible since as per the source (Kaggle) , the data was compressed using Principle Component Analysis (PCA) in order to protect the privacy of the individuals while making a realistic secnario dataset availaible to public .

# Data Preprocessing and Visualisation :
![](https://github.com/meghasolanki008/Credit_card_fraud_detection/blob/main/screenshots/data.png)

# Correlations :
![](https://github.com/meghasolanki008/Credit_card_fraud_detection/blob/main/screenshots/correlation.png)

The features are only correlated with the Class and time variables , hence it is a great indicator that simple models would be helpful here ,neural networks wont be needed hopefully .

# Relation between target variables and columns:
![](https://github.com/meghasolanki008/Credit_card_fraud_detection/blob/main/screenshots/lmplot.png)

A plot between different columns and amount along with different colours for target variable show that our output classes are separable by linear boundary , hence LOGISTIC REGRESSION can help in separating the multivariable data into 2 classes .

# Class Imbalance in dataset :
![](https://github.com/meghasolanki008/Credit_card_fraud_detection/blob/main/screenshots/unbalanced%20data.png)

This shows that we have way way less data for fraud cases than for non fraud cases , which is expected from the dataset .

To cure imbalance , we can use undersampling or oversampling . Here , I have decided to use SMOTE to counter the class imbalance in the dataset .

![](https://github.com/meghasolanki008/Credit_card_fraud_detection/blob/main/screenshots/SMOTE.png)

# Results from part 1:

![](https://github.com/meghasolanki008/Credit_card_fraud_detection/blob/main/screenshots/result%20part%201.png)

The F1 score came 0.99 meaning the Classifier is working great . It managed to catch 91 out of 101 frauds , thus preventing frauds 90% of the time . The confusion matrix , precision , recall and F1 score has been displayed for your convenience . The confusion matrix readings and the F1 show the success of the project .

# Results from part 2 :

Frauds are time independent so we can drop time :
![](https://github.com/meghasolanki008/Credit_card_fraud_detection/blob/main/screenshots/Transaction%20with%20time.png)

Lower Dimension Visualization is beautiful :

![](https://github.com/meghasolanki008/Credit_card_fraud_detection/blob/main/screenshots/dimensionality%20reduction.png)

I decided to undersample the dataset since significance of the data would be more realistic if there was no synthetic dataset. I also decided to choose the ML model with most recall , reason being that I realized later that as a business, labelling a Non Fraud datapoint as fraudulent would be much more worse for the company, since nobody would like their card to decline and people would literally stop using that credit card, so we must focus more on achieving lower recall than only blindly improving F1 score . So I got Logistic regression as the winner again with the following results :

![](https://github.com/meghasolanki008/Credit_card_fraud_detection/blob/main/screenshots/recall%20comparision.png)

Other models weren't much far behind regarding performance too , but I decided to keep the final code clean and keep the trial and error part in the "raw_code" file .

      

      
      
