# Modeling Car Insurance Claim Outcomes

Insurance companies invest a lot of time and money into optimizing their pricing and accurately estimating the likelihood that customers will make a claim. In many countries, having car insurance is a legal requirement to drive a vehicle on public roads, making the market very large!

On the Road Car Insurance has requested your services to build a model that predicts whether a customer will make a claim on their insurance during the policy period. They have asked you to identify the single feature that results in the best performing model, as measured by accuracy, so they can start with a simple model in production.

## Project Overview

The objective of this project is to analyze customer data from a CSV file called `car_insurance.csv` and identify the best predictor feature for whether a customer will file a claim, represented by the "outcome" column. The result will be stored in a DataFrame named `best_feature_df`, containing columns named "best_feature" and "best_accuracy".

## Dataset Description

The dataset `car_insurance.csv` contains the following columns:

| Column Name          | Description                                      | Data Type |
|----------------------|--------------------------------------------------|-----------|
| id                   | Unique identifier for each customer              | int64     |
| age                  | Age of the customer                              | int64     |
| gender               | Gender of the customer (1 = Male, 0 = Female)   | int64     |
| driving_experience   | Years of driving experience                       | object    |
| education            | Level of education (e.g., High School, College) | object    |
| income               | Income level of the customer                     | object    |
| credit_score         | Credit score of the customer                     | float64   |
| vehicle_ownership    | Vehicle ownership status (1 = Own, 0 = Lease)   | float64   |
| vehicle_year         | Year of the vehicle                              | object    |
| married              | Marital status (1 = Married, 0 = Not Married)   | float64   |
| children             | Number of children                               | float64   |
| postal_code          | Postal code of the customer                      | int64     |
| annual_mileage       | Annual mileage of the vehicle                    | float64   |
| vehicle_type         | Type of vehicle (e.g., SUV, Sedan)              | object    |
| speeding_violations  | Number of speeding violations                     | int64     |
| duis                 | Number of DUI violations                          | int64     |
| past_accidents       | Number of past accidents                         | int64     |
| outcome              | Whether the customer filed a claim (1 = Yes, 0 = No) | int64     |
