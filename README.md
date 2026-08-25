# Food Delivery Times Analysis and Prediction

## Overview

This project analyzes a food delivery dataset and uses machine learning models to predict delivery times.

The main goal is to understand the factors that influence delivery time and evaluate different regression models to determine which one provides the best predictions.

The project follows a typical Data Science workflow, including data exploration, data preprocessing, exploratory analysis, model training, and evaluation.

---

## Dataset

The dataset contains information about food deliveries, including characteristics related to the order, delivery, courier, weather, traffic, and other factors.

The target variable is:

*Delivery_Time_min* — the delivery time in minutes.

---

## Exploratory Data Analysis

The exploratory analysis includes:

- Dataset overview and structure
- Data types
- Missing value analysis
- Statistical summaries
- Distribution analysis
- Boxplots for numerical variables
- Analysis of categorical variables
- Correlation analysis
- Investigation of relationships between numerical features and delivery time

---

## Data Preprocessing

The dataset was prepared before model training.

### Categorical Features

Categorical variables were transformed into numerical representations using *One-Hot Encoding*.

---

## Machine Learning Models

Two regression models were initially trained and compared:

### Linear Regression

Linear Regression was selected because the exploratory analysis suggested approximately linear relationships between some predictors and delivery time.

### Random Forest Regressor

Random Forest was selected as a non-linear model capable of capturing more complex relationships between the features and the target variable.

---

## Model Evaluation

Because Delivery_Time_min is a continuous numerical variable, this is a *regression problem*.

The models were evaluated using:

### Mean Absolute Error (MAE)

Measures the average absolute difference between the actual and predicted delivery times.

It can be directly interpreted in minutes.

### Root Mean Squared Error (RMSE)

Measures the square root of the average squared prediction error.

RMSE gives greater weight to larger errors.

### R² Score

Measures how much of the variability in the target variable is explained by the model.

---

## Initial Results

The initial models produced the following results on the test set:

| Model | MAE (min) | RMSE (min) | R² |
|---|---:|---:|---:|
| Linear Regression | *7.087273* | *10.751675* | *0.747703* |
| Random Forest | 7.548116 | 11.647036 | 0.70393 |

Based on these initial results, *Linear Regression performed better than the initial Random Forest configuration* across all three evaluation metrics.

The Linear Regression model achieved an average prediction error of approximately *7.087273 minutes*.

---

## Prediction Analysis

In addition to numerical evaluation metrics, the project analyzes model predictions using:

- Actual vs. predicted delivery time plots

---

## Technologies

The project was developed using:

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab
- Git & GitHub

---
