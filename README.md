# Loan Status Prediction Project

## Overview
This project aims to predict loan status based on various financial metrics. We utilize a dataset from a lending company, which includes information such as credit score, annual income, and debt-to-income ratios, among others. The primary goal is to build a predictive model to accurately classify whether a loan will be paid off or will default.

## Data Preprocessing
The data was first loaded from a CSV file into a Pandas DataFrame. We then separated the dataset into features (`X`) and the target label (`y`), which is the loan status. The features include all columns except the target label. 

To address the imbalance in the dataset, we applied random oversampling using the `RandomOverSampler` from the imbalanced-learn library. This ensures that both classes in the target variable have an equal number of data points for the model training phase.

## Model Training and Evaluation
We used a logistic regression model for this classification task. The model was trained on both the original dataset and the resampled dataset to compare performance. Model evaluation was based on several metrics:
- Accuracy Score
- Balanced Accuracy Score
- Confusion Matrix
- Classification Report

### Logistic Regression with Original Data
First, we trained the logistic regression model using the original dataset and evaluated its performance.

### Logistic Regression with Resampled Data
Next, we trained another logistic regression model using the resampled (balanced) dataset to see if addressing the class imbalance would improve the model's performance.

## Results
The evaluation metrics showed that [briefly summarize the results, highlighting any significant improvements in model performance after resampling].

## Conclusion
This project demonstrates the importance of handling class imbalance in predictive modeling. By resampling the dataset to balance the classes, we were able to conclude that for both the Logistic Regression and Logistic Regression with Oversampled data model that the prediction for healthy loan was at 100% and for the oversampled data the prediction was 84%-85% respectively for the high-risk loan.


