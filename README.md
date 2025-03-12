# Credit-risk-classification

## Purpose of the Analysis

In this assignment we'll use several techniques to train and evaluate a model based on loan risk. We will use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Finantial information description

For the assignment we will use a dataset that contains this information:

![Screenshot 2025-03-11 at 9 25 39 p m](https://github.com/user-attachments/assets/99a72260-a1bc-4801-9281-e0de7b26436c)

As we can see this contains the principal information needed to evaluate the creditworthiness of borrowers such as
+ Loan size
+ Interest rate
+ Borrower income
+ Debt to income
+ Number of accounts
+ Derogatory Marks
+ Total Debt
+ Loan Status

## Information about the variable to predict

For the analysis the variable that we want to predict is the loan_status column in which `0` means a(healthy loan) and `1` a (high-risk loan)
So we will take that variable as the target variable for the analysis

## Stages of the Machine Learning Model

### Linear Regression Model

### Step 1

First we will implement a linear regression model 
The step number 1 is to separate the data into labels and features
1. Separate the y variable, the labels
2. Separate the X variable, the features

Our variables then will look like this:

![Screenshot 2025-03-11 at 9 32 21 p m](https://github.com/user-attachments/assets/27d1af7b-73ff-4b76-b136-1ced563c9627)

### Step 2

We will split the data into training and testing datasets by using `train_test_split`

### Step 3

We will fit a logistic regression model by using the training data (`X_train` and `y_train`) and save the predictions on the testing data labels by using the testing feature data (`X_test`) and the fitted model

### Step 4

We will Evaluate the model’s performance by doing the following:

* Generate a confusion matrix.
* Print the classification report.

For our linear regression model we obtained these results:

![Screenshot 2025-03-11 at 9 45 01 p m](https://github.com/user-attachments/assets/d12fb291-cc7e-4624-8290-0624694d5e97)

