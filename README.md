# Mileage Prediction Using Machine Learning

This project develops machine learning models to predict vehicle mileage (kmpl) based on engine and performance features such as displacement, horsepower, weight, and acceleration. The project implements both linear and polynomial regression techniques to analyze the relationships between these factors and provide accurate mileage estimates.

## Objective
The primary objective is to create a machine learning model that can predict a vehicle’s mileage (kmpl) using key features such as displacement, horsepower, weight, and acceleration. By building both linear and polynomial regression models, the project aims to find the model that best captures the relationships between these variables and provides more accurate mileage predictions.

## Dataset
The dataset contains several attributes related to vehicles, including:
- `kmpl`: Mileage (target variable)
- `cylinders`: Number of cylinders in the engine
- `displacement`: Engine displacement
- `horsepower`: Engine horsepower
- `weight`: Vehicle weight
- `acceleration`: Time taken to accelerate
- `model_year`: Year of manufacture
- `origin`: Origin of the vehicle
- `name`: Vehicle model

## Technologies Used
The following libraries and tools were used in this project:
- **Python** for programming
- **pandas** and **numpy** for data manipulation and numerical operations
- **matplotlib** and **seaborn** for data visualization
- **scikit-learn** for machine learning, specifically:
  - `LinearRegression`
  - `PolynomialFeatures`
  - `StandardScaler`
  - `train_test_split`

## Methodology
1. **Data Exploration**: Visualized the relationships between the target variable (kmpl) and predictors (displacement, horsepower, weight, and acceleration) to understand trends and correlations.
2. **Data Preprocessing**: Standardized the features using **StandardScaler** to ensure all variables are on the same scale.
3. **Train-Test Split**: Split the dataset into training and testing sets to evaluate the model's performance.

## Modeling
Two machine learning models were developed:
1. **Linear Regression**: Used to predict mileage assuming linear relationships between the predictors and the target variable.
2. **Polynomial Regression**: A higher-order regression model using **PolynomialFeatures** to capture non-linear relationships between the variables.

## Results
The performance of the linear and polynomial regression models was evaluated using several key metrics:

- **Linear Regression**:
  - Mean Absolute Error (MAE): 0.2561
  - Mean Absolute Percentage Error (MAPE): 14.73%
  - R² Score: 0.7021

- **Polynomial Regression**:
  - Mean Absolute Error (MAE): 0.2147
  - Mean Absolute Percentage Error (MAPE): 12.11%
  - R² Score: 0.7453

The polynomial regression model outperformed the linear regression model across all metrics, with lower errors and a higher R² score, indicating that it better captured the non-linear relationships between the predictors and mileage.

