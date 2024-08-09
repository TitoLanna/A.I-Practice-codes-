

# California Housing Price Prediction using Linear Regression

This repository contains a Python implementation of a linear regression model to predict California housing prices using the `scikit-learn` library and the California Housing dataset. The project demonstrates data fetching, preprocessing, model training, and evaluation with a simple linear regression model.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project aims to predict the median house value in California districts based on various features such as median income, house age, average number of rooms, and more. We use the California Housing dataset, fetched using `scikit-learn`, and implement a linear regression model to make predictions.

## Dataset

The California Housing dataset contains data from the 1990 U.S. Census, including information on median house values, median incomes, and other demographic details for various districts in California.

- **Number of Instances:** 20,640
- **Number of Attributes:** 8 numeric features and 1 target variable
- **Target Variable:** Median house value (in $100,000s)
- **Features:**
  - `MedInc`: Median income in block group
  - `HouseAge`: Median house age in block group
  - `AveRooms`: Average number of rooms per household
  - `AveBedrms`: Average number of bedrooms per household
  - `Population`: Block group population
  - `AveOccup`: Average number of household members
  - `Latitude`: Block group latitude
  - `Longitude`: Block group longitude

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/california-housing-prediction.git
    ```
2. Navigate to the project directory:
    ```bash
    cd california-housing-prediction
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

Run the Python script to fetch the data, split it into training and testing sets, train a linear regression model, and evaluate its performance:
```bash
python housing_price_prediction.py
```

## Code Explanation

### Data Fetching

The dataset is fetched using the `fetch_california_housing` function from `sklearn.datasets`.

### Data Splitting

The dataset is split into training and testing sets using the `train_test_split` function:
```python
X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=0.2)
```
- **Training Set:** 16,512 instances
- **Testing Set:** 4,128 instances

### Linear Regression Model

A linear regression model is implemented using `scikit-learn`'s `LinearRegression` class. The model is trained on the training data and evaluated on the test data.

### Model Evaluation

The model's performance is evaluated using the following metrics:
- **Coefficients**: Weight assigned to each feature by the model.
- **Intercept**: The bias term of the model.
- **Mean Squared Error (MSE)**: Measures the average squared difference between the predicted and actual values.
- **Coefficient of Determination (R²)**: Indicates the proportion of the variance in the target variable explained by the model.

## Results

The model's output includes the coefficients, intercept, MSE, and R² score. Example output:
```python
Coefficients: [ 4.298e-01  9.702e-03 -9.648e-02  5.975e-01 -5.919e-06 -9.121e-03 -4.241e-01 -4.368e-01]
Intercept: -37.07504229444323
Mean squared error (MSE): 0.53
Coefficient of determination (R²): 0.59
```

A scatter plot is also generated to visualize the relationship between the actual and predicted values.
