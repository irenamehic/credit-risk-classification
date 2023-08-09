# credit-risk-classification
In this challenge, we use various techniques to train and evaluate a model based on loan risk. The data set includes historical lending activity from a peer-to-peer lending services company, and can be accessed in the "Resources" folder from withitn the "Credit_Risk" folder.

 - - - Credit Risk Analysis Report - - -
Overview of the Analysis
The purpose of this analysis is to train and evaluate a model based on potential loan risk. The loan risk can be a useful model since it could identify the creditworthiness of borrowers.

The model will learn from these variables: loan_size, interest_rate, borrower_income, debt_to_income, num_accounts, derogatory_marks, total_debt and loan_status. Then, it will be tested to predict the variable loan_status, and determine if the borrower has a healthy loan (represented as 0), or a high-risk loan (represented as 1)

Stages of this machine learning process:

Data was split into Training Set and Testing Set:

The .csv data from the Resources folder is read into Pandas DataFrame.
Create a set from loan_status(y) and create a features(X) DataFrame with the remaining columns.
Then split the data into Training and Testing Sets.
A LogisticRegression model was created:

Fit the model using Training Set.

Score the model


Make predictions using the Testing Set and the Trained model

Score the model

A confusion matrix is generated and the classification report for the model is printed.

Results

Model on the Training Set:

Accuracy: 99%
Precision: 100% for Class 0, 86% for Class 1.
Recall: 100% for Class 0, 90% for Class 1.

Model on the Testing Set:

Accuracy: 99%
Precision: 100% for Class 0, 85% for Class 1.
Recall: 99% for Class 0, 91% for Class 1.

Summary
Looking at the two classification reports for the training and test data, it looks as if model performance declined slightly on the test data. However, we can expect to this type of slight deviation since this is how well the model is performing on data that the model hasn't seen before. If we're still getting strong precision and recall on the test dataset, this is a good indication about how well the model is likely to perform in real life. For example, if the lending company decides to use this model on unseen data for "Healthy-Loan" customer, they can expect to accurately predict those customers' loan risk (100%)
