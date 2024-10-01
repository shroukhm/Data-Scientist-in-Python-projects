# Predicting Movie Rental Durations

## Overview

In this project, we use regression models to predict the number of days a customer rents DVDs for. The dataset provided is a CSV file called `rental_info.csv`, which contains details about rental transactions. The objective is to preprocess the data, apply regression models, and recommend the model with the lowest mean squared error (MSE) on the test set.


## Dataset

The dataset `rental_info.csv` contains the following features:

- **rental_date**: The date and time the customer rented the DVD.
- **return_date**: The date and time the customer returned the DVD.
- **amount**: The amount paid by the customer for renting the DVD.
- **amount_2**: The square of `amount`.
- **rental_rate**: The rate at which the DVD was rented.
- **rental_rate_2**: The square of `rental_rate`.
- **release_year**: The release year of the rented movie.
- **length**: The length of the movie in minutes.
- **length_2**: The square of `length`.
- **replacement_cost**: The replacement cost of the DVD.
- **special_features**: The special features available on the DVD (e.g., "Deleted Scenes", "Behind the Scenes").
- **NC-17**, **PG**, **PG-13**, **R**: Dummy variables indicating the movie rating.


## Data Preprocessing

1. **Load Data**: Load `rental_info.csv` using `pandas`.
   
2. **Calculate Rental Length**: Create a new column `rental_length_days` by calculating the difference (in days) between `return_date` and `rental_date`. This will be the target variable.

3. **Dummy Variables**: Extract dummy variables from the `special_features` column:
   - `deleted_scenes`: Takes the value 1 if `special_features` contains "Deleted Scenes".
   - `behind_the_scenes`: Takes the value 1 if `special_features` contains "Behind the Scenes".

4. **Feature Matrix (X)**: Create a pandas DataFrame `X` containing all relevant features for model training, avoiding columns that leak information about the target (e.g., `rental_length_days`).

5. **Target Variable (y)**: Select `rental_length_days` as the target variable and store it as a pandas Series `y`.

## Model Training and Evaluation

- **Train-Test Split**: Split the data into training and test sets (`X_train`, `y_train`, `X_test`, `y_test`), using 20% of the data for testing. Set `random_state=9` to ensure reproducibility.

- **Regression Models**: Apply different regression models to the dataset.

- **Evaluation**: Use Mean Squared Error (MSE) to evaluate model performance, aiming for an MSE of less than 3 on the test set.

## Best Model

- Save the model with the lowest MSE as `best_model`.
- Save its corresponding MSE on the test set as `best_mse`.
