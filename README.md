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

## Linear Regression Model

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

![Screenshot 2025-03-11 at 10 11 58 p m](https://github.com/user-attachments/assets/05586f5c-5fe7-4db5-bfce-1b7e961ba962)


## Conclussions of linear regression model

**Question:** How well does the logistic regression model predict both the `0` (healthy loan) and `1` (high-risk loan) labels?

**Answer:** 
The model does a god job in identifying the healthy loans and high risk loans
As we can see on the confussion matrix we have a 18'658 results on predicted and actual positives and 582 cases on predicted negatives and actual negatives.

Also our classification reports tells us there's a precision of 84% so loans predicted as high risk got an almost 85% of accuracy in detecting them
The recall identified 94% of actual high risk loans with only 110 loans missed
The F1-Score indicated a good balance of precision and recall for high risk loans.

The overall performance gives us that we have a 99% accuracy telling us that it predicted correctly the loan status on most of the cases.
The macro average having a .92 tells us that maybe there is a level of unbalance in our data so we can take this into account.
And finally the weighted average reflects that the model performs very well overall.

## Random Forest Classifier Model

For this model we will follow these steps for the analysis

### Step 1

# Split the data into training and testing sets and scale the feature data 

### Step 2

Instantiate the Random Forest Classifier, Fit the model using the scaled training data and Make predictions using the testing data

### Step 3

Generate a confusion matrix for the Random Forest model and Print the classification report for the Random Forest model

For this model we obtained the following results

![Screenshot 2025-03-11 at 10 10 40 p m](https://github.com/user-attachments/assets/30bf01e5-eb58-4852-9da2-65bca1da8dcf)

## Conclussions of Random Forest Classifier



# Final Conclussions

















