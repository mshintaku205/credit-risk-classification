# Credit Risk Classification
Module 20 Challenge


## Project Description
Use various techniques to train and evaluate a model based on loan risk. A dataset of historical lending activity from a peer-to-peer lending services company is used to build a model that can identify the creditworthiness of borrowers.

## Preparation of the Analysis
1. Split the Data into Training and Testing Sets
2. Create a Logistic Regression Model with the Original Data
3. Write a Credit Risk Analysis Report


## 1. Split the Data into Training and Testing Sets
- Read the CSV data file into a Pandas DataFrame
- Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns
- Split the data into training and testing datasets

## 2. Create a Logistic Regression Model with the Original Data
- Fit a logistic regression model by using the training data (X_train and y_train)
- Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model
- Evaluate the model’s performance by generating a confusion matrix and printing the classification report
- See how well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

## 3. Write a Credit Risk Analysis Report
The logistic regression model performs well in predicting both healthy and high-risk loans, as demonstrated by its high accuracy score of 99.18% and balanced accuracy score of 95.20%. However, it is important to note that the dataset is imbalanced, with 96.77% of the target values (75,036 out of 77,536) representing healthy loans.

Due to the disproportionate representation of healthy loans in the data, the model is more likely to predict the status of healthy loans accurately compared to high-risk loans. This is evident in the classification report, where the model achieved 100% precision in predicting healthy loans ('0'), while it only correctly predicted high-risk loans ('1') 85% of the time.