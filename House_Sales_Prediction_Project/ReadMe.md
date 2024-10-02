# House Sales Prediction Project

## Project Overview

This project is focused on predicting house sale prices using a dataset of house sales. It involves cleaning the dataset, engineering features, and applying machine learning models to predict house prices.

## Data

The dataset contains records of previous houses sold in the area.

| Column Name  | Criteria |
|--------------|---------------------------------------------------------|
| `house_id`   | Nominal. Unique identifier for houses. Missing values not possible. |
| `city`       | Nominal. The city in which the house is located. One of 'Silvertown', 'Riverford', 'Teasdale', and 'Poppleton'. Replace missing values with "Unknown". |
| `sale_price` | Discrete. The sale price of the house in whole dollars. Values can be any positive number greater than or equal to zero. Remove missing entries. |
| `sale_date`  | Discrete. The date of the last sale of the house. Replace missing values with "2023-01-01". |
| `months_listed` | Continuous. The number of months the house was listed on the market prior to its last sale, rounded to one decimal place. Replace missing values with mean number of months listed, to one decimal place. |
| `bedrooms`   | Discrete. The number of bedrooms in the house. Any positive values greater than or equal to zero. Replace missing values with the mean number of bedrooms, rounded to the nearest integer. |
| `house_type` | Ordinal. One of "Terraced" (two shared walls), "Semi-detached" (one shared wall), or "Detached" (no shared walls). Replace missing values with the most common house type. |
| `area`       | Continuous. The area of the house in square meters, rounded to one decimal place. Replace missing values with the mean, rounded to one decimal place. |


## Project Steps

1. **Data Cleaning**:
    - Handled missing values:
        - `city`: Replaced missing values with `"Unknown"`.
        - `sale_price`: Rows with missing `sale_price` were removed.
        - `sale_date`: Missing values were replaced with `"2023-01-01"`.
        - `months_listed`: Replaced missing values with the mean, rounded to one decimal place.
        - `bedrooms`: Missing values were replaced with the mean, rounded to the nearest integer.
        - `house_type`: Missing values were replaced with the most common house type.

2. **Feature Engineering**:
    - Categorical features were converted into dummy variables to prepare the dataset for machine learning models.

3. **Modeling**:
    - A `RandomForestRegressor` model was used for prediction.
    - A `LinearRegression` model was used for prediction.
    - The model was trained on the cleaned dataset, and predictions were generated for the validation set.

4. **Output**:
    - The final output is a DataFrame containing the `house_id` and the predicted `price` for each house in the validation dataset.
