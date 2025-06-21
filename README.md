# Project-4---Diabetes-Prediction-Test
This repository implements a supervised classification pipeline to predict the onset of diabetes using patient health metrics. Leveraging the Pima Indians Diabetes dataset, the workflow comprises:

Data Ingestion & Cleaning
Load demographic and medical measurements (e.g., glucose, blood pressure, BMI), replace physiologically invalid zeros via imputation, and remove duplicate records.

Exploratory Data Analysis (EDA)
Visualize feature distributions with histograms and boxplots, examine inter-feature relationships via a correlation heatmap, and assess the class balance of the binary target (Outcome).

Feature Engineering & Preprocessing
Impute missing or invalid entries and, where appropriate, create interaction features to capture non-linear effects.

Model Development
Four classifiers are trained on an 80/20 train–test split without additional automated hyperparameter searches:

Logistic Regression (baseline)

CatBoost Classifier

LightGBM Classifier

Random Forest Classifier

Evaluation
Models are compared using Accuracy, F1 score, and ROC-AUC. Confusion matrices and ROC curves visualize class-specific performance and trade-offs.

Key Finding
The Random Forest Classifier achieved the highest overall performance, delivering the best balance of sensitivity and specificity on the held-out test set.

This notebook serves as an end-to-end tutorial for binary classification on structured health data, demonstrating best practices in data cleaning, feature preparation, and model assessment using Python’s scientific stack.

F1 Score and Accuracy Scores vs Models:
![Screenshot 2025-06-22 011601](https://github.com/user-attachments/assets/12a158bc-24fd-4d2b-96a7-5c86698117dd)
