# CodSoft Task 3: Sales Prediction Using Python

## Overview

This project aims to build a machine learning model to predict sales based on advertising expenditure across different platforms, such as TV, Radio, and Newspapers. By analyzing advertising data, the objective is to develop a model that forecasts sales and helps businesses optimize their advertising strategies for maximum impact.

## Dataset

The dataset used in this project contains information about advertising expenses and corresponding sales figures. It includes features like `TV`, `Radio`, `Newspaper`, and `Sales`. The dataset was provided in CSV format and underwent various preprocessing steps to prepare it for modeling.

### Dataset Columns:
- **TV**: Advertising budget spent on TV ads (in thousands).
- **Radio**: Advertising budget spent on radio ads (in thousands).
- **Newspaper**: Advertising budget spent on newspaper ads (in thousands).
- **Sales**: Sales generated as a result of the advertising (in thousands).

## Project Structure

### Data Preprocessing

- **Handling Missing Values**: The dataset was checked for missing values, and appropriate methods such as filling with mean values were applied.
- **Feature Scaling**: The dataset was explored to ensure consistent feature scaling, although normalization was not necessary due to the nature of the data.
- **Data Splitting**: The dataset was split into training and testing sets using an 80/20 split ratio.

### Feature Engineering

- **No additional feature engineering was necessary**: All features provided (TV, Radio, Newspaper) were used directly as input variables for the model.

### Modeling

- **Model Choice**: A Linear Regression model was employed to predict the target variable (`Sales`).
- **Training and Testing**: The model was trained on the training set and tested on unseen data using the testing set.

### Evaluation

- **Metrics**: The performance of the model was assessed using the following evaluation metrics:
  - **Mean Squared Error (MSE)**: Measures the average squared difference between actual and predicted sales.
  - **R-squared (R²)**: Explains the proportion of variance in the target variable that can be predicted from the independent variables.

## Model and Results

The Linear Regression model was trained and evaluated on the dataset. The performance metrics are as follows:

- **Mean Squared Error (MSE)**: The model achieved an MSE of approximately 2.907756910271091.
- **R-squared (R²)**: The R² score of the model was approximately 0.9059011844150826.

### Visual Results

A scatter plot of **Actual Sales vs. Predicted Sales** was generated to visually inspect the model’s performance. This visualization helps identify how well the model predicts sales based on the advertising budgets for TV, Radio, and Newspaper.

## Insights

The Linear Regression model provides a solid baseline for sales prediction based on advertising data. It successfully identifies relationships between different advertising channels and sales figures. There is potential for further improvements by experimenting with more complex models or introducing additional features that capture other factors affecting sales, such as seasonality or market trends.
