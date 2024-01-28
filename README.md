# LoanPrediction
Loan Default Prediction
# Loan Default Prediction

Welcome to the repository for my solution to the loan default prediction problem using a Random Forest Classifier. In this project, I aimed to predict which borrowers in the "test.csv" dataset are likely to default on their loans based on patterns identified in the "train.csv" dataset.

## Data:

- **train.csv:** Contains information about 255,347 borrowers, including loan details and whether they defaulted (ground truth).
- **test.csv:** Similar to train.csv but for 109,435 borrowers without the default information (target variable).

## Solution:

I implemented a machine learning pipeline to address the loan default prediction problem. Here's a breakdown of the key steps involved:

### Data Preprocessing:

- Cleaned and prepared the data for analysis, handling missing values, outliers, and feature engineering.
- Introduced two new features: 'CreditIncomeRatio' and 'LoanToIncomeRatio' based on existing features.
- Utilized one-hot encoding to convert the categorical feature 'LoanPurpose' into binary columns.
- Filled missing values with the mean of each column.

### Model Training:

- Employed a Random Forest Classifier with 100 trees and a maximum depth of 10 for training.
- Split the training data into training and validation sets using the `train_test_split` method.

### Model Evaluation:

- Assessed the model's performance on the validation set using the ROC AUC score.

### Prediction on Test Data:

- Used the trained model to predict default probabilities for each borrower in the "test.csv" dataset.
- Saved the predictions along with the corresponding loan IDs to a CSV file named "prediction_submission.csv".

## Results:

The Random Forest Classifier demonstrated promising results in predicting loan defaults for a significant portion of borrowers in the validation set.

## Sharing the Code:

This repository includes the Python script and Jupyter notebook containing the detailed code for data preprocessing, model training, evaluation, and prediction. Feel free to explore and build upon this solution for further enhancements.

Happy coding!
