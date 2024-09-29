# # Hypothesis Testing with men's and women's Soccer Matches


## Project Overview

This project aims to perform a hypothesis test to determine whether the mean number of goals scored in women's international soccer matches is the same as that in men's matches. The analysis focuses on official FIFA World Cup matches since January 1, 2002, and uses a 10% significance level.


## Objective

The primary research question is:

> **Are more goals scored in women's international soccer matches than in men's?**

## Hypotheses

- Null Hypothesis (H_0): The mean number of goals scored in women's international soccer matches is the same as in men's.
- Alternative Hypothesis (H_A): The mean number of goals scored in women's international soccer matches is greater than in men's.

## Data Sources

The analysis utilizes two datasets containing the results of every official men's and women's international football match since the 19th century. The data is stored in two CSV files:

- `women_results.csv`: Contains results of women's international matches.
- `men_results.csv`: Contains results of men's international matches.

These datasets were scraped from reliable online sources.

## Methodology

1. **Data Loading**: Load the datasets and filter the results to include only official FIFA World Cup matches since January 1, 2002.
2. **Hypothesis Testing**: Conduct an appropriate statistical hypothesis test to determine the p-value.
3. **Result Storage**: Store the p-value and the result of the test (either "reject" or "fail to reject") in a dictionary named `result_dict`.
