# Donor Discovery

This project evaluates various supervised learning algorithms to model individuals' income using data from the 1994 U.S. Census. The primary objective is to predict whether a person earns more than $50,000 annually, aiding non-profit organizations in identifying potential donors and optimizing their donation solicitation strategies.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Preprocessing](#data-preprocessing)
- [Model Evaluation](#model-evaluation)
- [Model Tuning](#model-tuning)
- [Results](#results)

## Introduction

Understanding the income levels of potential donors is critical for non-profit organizations. This project aims to build a model that accurately predicts whether an individual earns more than $50,000 annually using census data. The model's predictions help non-profits make informed decisions about whom to approach and what donation amounts to request.

## Dataset

The dataset used in this project comes from the UCI Machine Learning Repository and includes data from the 1994 U.S. Census. The original dataset was modified by:
- Excluding the 'fnlwgt' feature.
- Removing records with missing or poorly formatted entries.

## Exploratory Data Analysis

Initial analysis was performed to understand the distribution of features and their relationship with the target variable (`income`):
- Descriptive statistics provided insights into the data distribution.
- Visualizations helped understand the relationship between features and income.

## Data Preprocessing

Data preprocessing steps included:
1. Handling missing values and erroneous entries.
2. Transforming skewed continuous features using log transformation.
3. Normalizing numerical features.
4. Converting categorical features into numerical values using one-hot encoding.
5. Encoding the target variable (`income`) as binary values.

## Model Evaluation

The following supervised learning algorithms were evaluated:
1. Decision Trees
2. Support Vector Machines (SVM)
3. Ensemble Methods: AdaBoost
4. Logistic Regression
5. K-Nearest Neighbors (KNN)
6. Random Forest

Each model's performance was assessed using accuracy and F-beta score, with emphasis on precision.

## Model Tuning

AdaBoost was further tuned using GridSearchCV to optimize parameters like `n_estimators` and `learning_rate`, along with parameters of the base estimator (Decision Tree).

## Results

The tuned AdaBoost model provided the best accuracy and F-beta score, making it the most suitable model for this problem.



