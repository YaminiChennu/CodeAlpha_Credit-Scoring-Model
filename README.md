## Credit Scoring Model
## Project Overview
This project develops a Credit Scoring Model to predict the creditworthiness of individuals based on their historical financial data. The primary objective is to classify individuals as either likely to default or not default using various classification algorithms and evaluating their performance. The model uses historical financial data to train and test its predictions.

## Dataset
The dataset used in this project contains historical financial information about individuals. It includes features like:

DerogCnt: Count of derogatory remarks.
CollectCnt: Count of collections.
BanruptcyInd: Indicator for bankruptcy.
InqCnt06: Number of inquiries in the last 6 months.
TLBalHCPct: Total loan balance to high credit percentage.
TLDel90Cnt24: Number of delinquencies over 90 days in the last 24 months.
The target variable (TARGET) indicates whether the individual is likely to default (1) or not (0).

## Steps
## 1. Data Preprocessing
Drop irrelevant columns (e.g., ID).
Handle missing values by filling with the mean.
Split the dataset into training and test sets.
Standardize the feature set using StandardScaler.
## 2. Model Development
We trained multiple classification models to predict creditworthiness:

Logistic Regression
Decision Tree
Random Forest
Support Vector Machine (SVM)
## 3. Evaluation Metrics
Several metrics were used to assess the performance of the models:

Accuracy: The percentage of correct predictions.
Precision: The ability of the model to avoid false positives.
Recall: The ability of the model to find all true positives.
F1-Score: A weighted average of precision and recall.
AUC-ROC: Measures the model's ability to distinguish between classes.
## 4. Feature Importance
Random Forest: Feature importance scores to assess which features contribute most to creditworthiness.
Logistic Regression: Coefficients are used to understand the impact of each feature.
## 5. Cross-Validation
To ensure the robustness of the models, k-fold cross-validation was performed. This technique splits the data into k subsets and trains the model k times, each time using a different subset as the test set.

## 6. Handling Imbalanced Data
If the dataset is imbalanced (i.e., more default or non-default records), we used class weighting in Logistic Regression to adjust for the imbalance.
## Results
# Logistic Regression:

Accuracy: 85%
Precision: 80%
Recall: 78%
F1-Score: 79%
AUC-ROC: 0.87
# Random Forest:

Accuracy: 88%
Precision: 83%
Recall: 82%
F1-Score: 83%
AUC-ROC: 0.90
# Support Vector Machine:

Accuracy: 86%
Precision: 81%
Recall: 80%
F1-Score: 80%
AUC-ROC: 0.89
