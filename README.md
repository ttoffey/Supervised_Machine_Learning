# Supervised_Machine_Learning - Predicting Credit Risk


## Objective 
Build a machine learning model that attempts to predict whether a loan from LendingClub will become high risk or not. 

### Background

LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API.

Using this data, create machine learning models to classify the risk level of given loans. Specifically, you will be comparing the Logistic Regression model and Random Forest Classifier.

### Retrieve the data

An entire year's worth of data (2019) to predict the credit risk of loans from the first quarter of the next year (2020).* 

* `2019loans.csv`
* `2020Q1loans.csv`

*Note: These two CSVs have been undersampled to give an even number of high risk and low risk loans. In the original dataset, only 2.2% of loans are categorized as high risk. To get a truly accurate model, special techniques need to be used on imbalanced data. Undersampling is one of those techniques. Oversampling and SMOTE (Synthetic Minority Over-sampling Technique) are other techniques that are also used.


## Models Used & Projections

RandomForestClassifier Model will be better than LogisticRegression due to the high number of features in the datasets.  

## Fit a LogisticRegression model and RandomForestClassifier model

Tried this two different ways. I set up the 2019 data as the training set (X_train and y_train) and set up the 2020 data as the testing set (X_test, y_test). The results were not great. Used unscaled and scaled data for both models - scaling the data improved the results. The RandomForestClassifier model did have better results than the LogisticRegression model on both unscaled and scaled datasets.

Tried merging the datasets which produced better results than above. Used unscaled and scaled data for both models and scaled data improved the results. Again, the RandomForestClassifer had better results than the LogisticRegression model on both unscaled and scaled datasets.

I think the RandomForestClassifer model had better results due to the number of features in the datasets. 


### References

LendingClub (2019-2020) _Loan Stats_. Retrieved from: [https://resources.lendingclub.com/](https://resources.lendingclub.com/)

- - -

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
