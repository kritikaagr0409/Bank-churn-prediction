# Churn Modelling Project

This project involves the analysis and prediction of customer churn using a dataset containing 10,000 records. The dataset includes customer demographics, account details, and churn status.

## Table of Contents
- [Overview](#overview)
- [Dataset Information](#dataset-information)
- [Project Structure](#project-structure)
- [Data Preprocessing](#data-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Technologies Used](#technologies-used)
- [Installation](#installation)

## Overview
The goal of this project is to build a predictive model that can identify whether a customer is likely to churn. We used Python and popular data analysis and machine learning libraries to preprocess data, build, and evaluate a Support Vector Classifier (SVC) model.

## Dataset Information
- *Source*: The dataset used in this project contains information on customer demographics, credit scores, account balances, and activity.
- *Features*: 13 columns including Geography, Gender, CreditScore, Age, Balance, etc.
- *Target*: Exited - a binary variable indicating whether the customer has churned (1) or not (0).

## Project Structure
1. *Data Loading*: Loading the data using Pandas.
2. *Exploratory Data Analysis (EDA)*: Analyzing categorical and numerical features using visualizations.
3. *Data Preprocessing*:
   - One-hot encoding for Geography
   - Label encoding for Gender
   - Dropping unnecessary columns like RowNumber, CustomerId, and Surname
4. *Feature Engineering*:
   - Creating custom classes FeatureEncoder, FeatureLabel, and FeatureDropper for data transformations.
5. *Modeling*:
   - Splitting the data into training and testing sets.
   - Standardizing features using StandardScaler.
   - Training an SVM model with an RBF kernel.
6. *Evaluation*:
   - Generating a classification report and calculating the accuracy score.

## Data Preprocessing
### Categorical Features Analysis
```python
def catagorical(df):
    ...
