# Data Transformation Project

## Project Overview
This project focuses on transforming a dataset for **Training Data Ltd.** to create an optimized DataFrame called `ds_jobs_transformed` that efficiently stores job-related data from the file `customer_train.csv`. The goal is to optimize memory usage by transforming the data types of various columns based on specific guidelines provided by the Head Data Scientist.

## Objective
The objective of this project is to:
- Transform the original dataset to store the data more efficiently by using appropriate data types.
- Filter the dataset to focus on professionals with substantial experience working in large companies.

## Requirements
The transformation must follow these specific requirements:

1. **Boolean Columns**:
   - Any column containing **two categories** should be stored as a Boolean (`bool`) type.

2. **Integer Columns**:
   - Any column containing **only integer values** must be stored as 32-bit integers (`int32`).

3. **Float Columns**:
   - Any column containing **float values** should be stored as 16-bit floats (`float16`).

4. **Nominal Categorical Data**:
   - Columns with **nominal categorical data** (unordered categories) must be stored as the `category` data type.

5. **Ordinal Categorical Data**:
   - Columns with **ordinal categorical data** (ordered categories) must be stored as ordered categories, reflecting the natural order of the values.

6. **Filtering**:
   - The resulting DataFrame should only include rows where:
     - The student has **10 or more years of experience**.
     - The company has **at least 1000 employees**.
