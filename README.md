# California-Housing-Regression-Analysis
This repository contains a regression analysis of the California Housing dataset using multiple machine learning algorithms. The project includes data preprocessing, model implementation, performance evaluation, and comparison of different regression models.
## Overview
This project performs regression analysis on the California Housing dataset using various machine learning algorithms. The goal is to compare different regression models based on their performance metrics and identify the best-performing model.

## Dataset

The dataset is fetched using fetch_california_housing from Scikit-Learn. It contains information about California housing prices based on features like median income, house age, and location.

## Preprocessing Steps

Load the dataset and convert it into a Pandas DataFrame.

Check for missing values and handle them appropriately. The dataset does not contain missing values, so no imputation was necessary.

Split the dataset into training (80%) and testing (20%) sets to evaluate model performance on unseen data.

Feature Scaling: Standardization is applied using StandardScaler to ensure that all features have the same scale. This is particularly important for algorithms like Support Vector Regressor (SVR) and Gradient Boosting Regressor that are sensitive to feature magnitudes.

### Justification for Preprocessing Steps

Checking for missing values ensures that models do not encounter errors due to missing data.

Splitting the dataset helps in training and validating the models properly.

Feature scaling improves model convergence and performance, especially for distance-based models like SVR.

## Regression Models Implemented

### Linear Regression

How it works: Linear Regression finds the best-fitting line by minimizing the sum of squared residuals.

Suitability: It is simple and provides a baseline model for comparison.

### Decision Tree Regressor

How it works: It splits the data into branches using decision rules to make predictions.

Suitability: Handles non-linear relationships well and is easy to interpret.

### Random Forest Regressor

How it works: Uses multiple decision trees and averages their outputs to improve accuracy and reduce overfitting.

Suitability: Works well for complex datasets with high variance.

### Gradient Boosting Regressor

How it works: Builds models sequentially, correcting errors from previous models using a boosting technique.

Suitability: Provides strong predictive performance, especially for structured data.

### Support Vector Regressor (SVR)

How it works: Uses support vectors and kernel functions to transform data into higher dimensions for better regression.

Suitability: Effective for datasets with complex relationships and requires feature scaling.

## Evaluation Metrics

The models are evaluated based on the following metrics:

### Mean Squared Error (MSE)

### Mean Absolute Error (MAE)

### R-squared Score (R²)

Results

The results are stored in a DataFrame and compared to determine the best and worst-performing models.
