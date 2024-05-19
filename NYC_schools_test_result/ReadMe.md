# Analyzing the performance of NYC schools

## Overview

Every year, American high school students take the SATs, which are standardized tests designed to assess literacy, numeracy, and writing skills. The SAT comprises three sections - reading, math, and writing - each with a maximum score of 800 points. These scores are crucial for students as they significantly influence college admissions decisions.

## Purpose

The goal of this analysis is to evaluate the performance of New York City (NYC) public schools on the SAT. This analysis is valuable for various stakeholders including policy and education professionals, researchers, government officials, and parents. By understanding school performance, stakeholders can make informed decisions and implement strategies to improve educational outcomes.


## Dataset

The dataset provided is schools.csv, which contains information about the SAT performance of NYC public schools. The dataset includes the following columns:

| columns         | description                                 |
|----------------|----------------------------------------------|
| **School Name**| The name of the school                       |
| **Borough**    | The NYC borough where the school is located  |
| **SAT Reading**| The average SAT reading score for the school |
| **SAT Math**   | The average SAT math score for the school    |
| **SAT Writing**| The average SAT writing score for the school |
| **Building Code**| The unique building code assigned to each school |
| **Percent Test**| The percentage of students who took the SAT at each school |




## Key Questions


1. **Which NYC schools have the best math results?**
   - Criteria: Schools with math results that are at least 80% of the maximum possible score of 800 (i.e., a score of 640 or higher).

2. **What are the top 10 performing schools based on the combined SAT scores?**
   - Criteria: The combined SAT score is the sum of the reading, math, and writing scores for each school.

3. **Which single borough has the largest standard deviation in the combined SAT score?**
   - Criteria: Calculate the standard deviation of the combined SAT scores for each borough and identify the one with the highest value.

## Methodology
To answer these questions, the following steps will be taken:
1. Load and inspect the dataset to understand its structure and content.
2. Identify schools with the best math results by filtering schools with an average math score of 640 or higher.
3. Calculate the combined SAT scores for each school and sort them to determine the top 10 performing schools.
4. Calculate the standard deviation of the combined SAT scores for each borough and identify the borough with the largest standard deviation.

### Usage
This analysis can be used to identify high-performing schools and understand variations in school performance across different NYC boroughs. The results can inform decisions related to policy-making, resource allocation, and school selection for parents.

