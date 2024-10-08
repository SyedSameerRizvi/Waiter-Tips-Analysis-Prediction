# Waiter Tips Prediction
This project aims to predict the tips given to waiters in a restaurant based on various factors such as total bill, gender, number of people, day of the week, and other demographic details. The primary objective is to develop a model that accurately predicts the tip amount using the available features.

## Project Overview
Tipping waiters depends on several factors such as the total bill amount, the number of people at the table, and demographic factors like gender. This project explores these relationships and builds a predictive model to estimate the tips based on these variables.

## Dataset
The dataset used is `tips.csv`, which contains the following features:

- total_bill: Total bill in dollars (including tax).
- tip: Tip amount given to the waiter (target variable).
- sex: Gender of the person paying the bill.
- smoker: Whether the person is a smoker.
- day: Day of the week (e.g., Sun, Sat).
- time: Time of the meal (Lunch or Dinner).
- size: Number of people at the table.

## Installation
Install the required dependencies:
  ```bash
      pip install -r requirements.txt
  ```

## Usage
1. Load the data and explore it:
 ```python
      import pandas as pd
      df = pd.read_csv("tips.csv")
      df.head()
  ```

2. Train a linear regression model using the available features to predict the tip amount:
```python
     from sklearn.linear_model import LinearRegression
     model = LinearRegression()
     model.fit(X_train, y_train)
  ```

## Model and Evaluation
The model chosen for this project is **Linear Regression**, given the continuous nature of the target variable (tip amount).

### Metrics:
- Mean Absolute Error (MAE): Measures the average magnitude of the errors in predictions.
- Mean Squared Error (MSE): Captures the difference between actual and predicted tips.
- R-squared (R²): Determines the proportion of variance explained by the features.
