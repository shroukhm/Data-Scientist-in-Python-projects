# Predictive Modeling for Agriculture

Measuring essential soil metrics such as nitrogen, phosphorus, potassium levels, and pH value is an important aspect of assessing soil condition. However, it can be an expensive and time-consuming process, which can cause farmers to prioritize which metrics to measure based on their budget constraints.

Farmers have various options when it comes to deciding which crop to plant each season. Their primary objective is to maximize the yield of their crops, taking into account different factors. One crucial factor that affects crop growth is the condition of the soil in the field, which can be assessed by measuring basic elements such as nitrogen and potassium levels. Each crop has an ideal soil condition that ensures optimal growth and maximum yield.

A farmer reached out to you as a machine learning expert for assistance in selecting the best crop for his field. They've provided you with a dataset called `soil_measures.csv`, which contains:

- `"N"`: Nitrogen content ratio in the soil
- `"P"`: Phosphorous content ratio in the soil
- `"K"`: Potassium content ratio in the soil
- `"pH"`: pH value of the soil
- `"crop"`: Categorical values that contain various crops (target variable)

Each row in this dataset represents various measures of the soil in a particular field. Based on these measurements, the crop specified in the `"crop"` column is the optimal choice for that field.  

## Project Overview

The objective of this project is to identify the single feature that has the strongest predictive performance for classifying crop types in the provided dataset. From this information, we will create a variable called `best_predictive_feature`, which will be a dictionary containing the best predictive feature name as a key and the evaluation score (for the metric you choose) as the value.

## Dataset Description

The dataset `soil_measures.csv` contains the following columns:

| Column Name | Description                                      | Data Type |
|-------------|--------------------------------------------------|-----------|
| N           | Nitrogen content ratio in the soil              | float     |
| P           | Phosphorous content ratio in the soil           | float     |
| K           | Potassium content ratio in the soil              | float     |
| pH          | pH value of the soil                            | float     |
| crop        | Categorical values representing various crops    | object    |
