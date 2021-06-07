# 11_Machine_Learning_HW

## Background

Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, a client has asked that you help them predict credit risk with machine learning techniques.

In this assignment you will build and evaluate several machine learning models to predict credit risk using data you'd typically see from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so you will need to employ different techniques for training and evaluating models with imbalanced classes. You will use the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:


### Resampling

I used the imbalanced learn library to resample the LendingClub data and build logisitic regression classifies using resampled data. After splitting the data into training and testing sets, I scaled the data using the `StandardScaler` from `sklearn.preprocessing`. 
I found/displayed the balanced accuracy score, confusion matrix and imbalanced classification report.
I also:
1. Oversampled the data using the `Naive Random Oversampler` and `SMOTE` algorithms.
2. Undersample the data using the `Cluster Centroids` algorithm.
3. Over- and undersample using a combination `SMOTEENN` algorithm.

I found/displayed the balanced accuracy score, confusion matrix and imbalanced classification report to compare all the models.

### Ensemble Learning

In this section, I trained and compared two different ensemble classifiers to predict loan risk and evaluate each model.
I used the Balanced Random Forest Classifier and the Easy Ensemble Classifier.
I used the balanced accuracy score, confusion matrix, and classification reports to compare both models.
