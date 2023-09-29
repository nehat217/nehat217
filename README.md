# Apartment Price Prediction README

This repository contains code for predicting apartment prices using machine learning techniques. The project includes data preprocessing, exploratory data analysis, model building, hyperparameter tuning, and evaluation.

## Data

The dataset used for this project is the "apartments_for_rent_classified_10K" dataset, which includes information about apartments for rent. The dataset contains the following columns:

- `amenities_count`: Count of amenities available in the apartment.
- `bathrooms`: Number of bathrooms in the apartment.
- `bedrooms`: Number of bedrooms in the apartment.
- `pets_allowed`: Whether pets are allowed in the apartment (binary feature).
- `price`: Rental price of the apartment (target variable).
- `square_feet`: Area of the apartment in square feet.
- `region`: The region where the apartment is located.

## Data Preprocessing

Data preprocessing steps include handling missing values, removing duplicates, encoding categorical variables, and scaling numerical features. The `state` column is mapped to a `region` column for better feature representation.

## Exploratory Data Analysis (EDA)

EDA involves data visualization using libraries like Seaborn and Matplotlib. Various plots and analyses are performed to understand the data distribution, correlations, and relationships between features and the target variable.

## Model Building

A linear regression model is built to predict apartment prices. The `SGDRegressor` from Scikit-Learn is used as the base model. The model is initially trained with default hyperparameters and evaluated.

## Hyperparameter Tuning

Hyperparameter tuning is performed using Randomized Search Cross-Validation. Different combinations of hyperparameters are explored to find the best-performing model in terms of root mean squared error (RMSE).

## Model Evaluation

The model is evaluated using RMSE and R-squared (R2) metrics on both the training and test datasets. The evaluation results are displayed, and a hyperparameter tuning plot is generated to visualize the impact of hyperparameters on model performance.

## OLS Model (Optional)

A model is built using the `statsmodels` library for a more detailed statistical summary.

## Repository Structure

The repository is organized as follows:

- CS4372HW1.py: Python script for predicting apartment prices.
- `README.md`: This README file providing an overview of the project.

## Dependencies

The following Python libraries are used in this project:

- NumPy
- Matplotlib
- Pandas
- Seaborn
- Scikit-Learn
- StatsModels

You can install these libraries using `pip install` if they are not already installed.

## How to Run

Install all dependencies above.  Open your terminal or command prompt and navigate to the directory where CS4372HW1.py is located. 

Execute the script using the Python interpreter: python apartment_price_prediction.py

Please note that this project requires an internet connection to access the dataset from the provided URL.
URL = "https://raw.githubusercontent.com/nehat217/nehat217/main/apartments_for_rent_classified_10K.csv"
