Customer Data Preprocessing Pipeline
 Overview

This project demonstrates a complete data preprocessing pipeline using Python. The dataset contains missing values, duplicates, categorical variables, and numerical features with different scales. The goal is to clean and prepare the data for machine learning models.

 Problem Statement

Given a raw customer dataset:

Handle missing values
Remove duplicate records
Encode categorical features
Scale numerical features
 Technologies Used
Python 
Pandas
NumPy
Scikit-learn
 Dataset Description
Column Name	Description
customer_id	Unique customer ID
age	Customer age (may be null)
city	Customer city (categorical)
gender	Male/Female
annual_income	Income in INR
 Tasks Performed
Task 1 — Data Cleaning
Missing values handled:
age → filled with median
city → filled with mode
Duplicate rows removed
Task 2 — Encoding
city → One-Hot Encoding
gender → Label Encoding
 Task 3 — Feature Scaling

Applied two scaling techniques:

 Min-Max Scaling
Scales data between 0 and 1
 Standardisation (Z-score)
Transforms data to:
Mean = 0
Standard Deviation = 1
When to Use What?
Min-Max Scaling
When data needs to be in a fixed range (0–1)
Used in KNN, Neural Networks
Standardisation
When data has outliers
Used in Linear Regression, SVM
