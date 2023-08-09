* Explain the purpose of the analysis.

The purpose of the analysis in to predict the creditworthiness of borrowers based on historical data. Specifically, the goal is to build a model that can accurately classify whether a potential borrower poses a high risk (is likely to default or not repay the loan) or low risk (is likely to repay the loan).


* Data description

Loan Size: This represents the amount of the loan.

Interest Rate: This is the rate charged by the lender. 

Borrower Income: Income levels.

Debt to Income Ratio: Measure used in credit scoring.

Number of Accounts: Number of accounts. 

Derogatory Marks: These are negative marks on a borrower's credit report.

Total Debt: This represents the total amount the borrower owes.

Waht was to be determined is whether a loan to the borrower in the testing set would be low- or high-risk 


* The primary variable that was predicted was loan_status which is a categorical variable that represents whether a loan is high risk or low risk. This variable was used as a classification label on the model.

* Stages of the machine learning process:

- Separate data into features X and the target variable y. The features, stored in 'X', are the columns used to make predictions about the loan status. The target variable 'y', is the actual loan status was the target to be predicted.

- Displayed the first few rows and labels to ensure that they are correctly separated.

- In order to understand the distribution of the target variable, the count the number of occurrences of each class i 'y' data using the value_counts() function. This gives an idea of whether the data is balanced or not.

- Split the data into training and testing sets using the train_test_split(). This is to ensure that a separate set of data to evaluate the model's performance after training.

- Create an instance of a logistic regression model using the LogisticRegression() function. For predicting whether a loan is high risk or low risk.

- Fit this logistic regression model to the training data. To learn the relationship between the features and the target variable, which allows the model to make predictions on unseen dat

- Predict the loan status on the testing data. Passing the test features to the predict() method of the trained model, which returns predicted labels for each data point.

- Confusion matrix of the model's predictions using the confusion_matrix() function. This gives a summary of how well your model is performing by showing the number of true positives, false positives, true negatives, and false negatives.



## Results

Machine Learning Model 1:
Summary of Model 1's Performance Metrics.
Using the original dataset, Model 1 achieved an impressive accuracy rate of 94.4% for the two classifications. For healthy loans, its precision and recall are impeccable, both at 1.00. On the other hand, when it comes to the high-risk loans, there's room for enhancement. The model correctly identified 87% of them, as reflected by the 0.87 precision rate. Moreover, out of all the high-risk loans in the dataset, the model spotted 89% of them, as indicated by the 0.89 recall score.
