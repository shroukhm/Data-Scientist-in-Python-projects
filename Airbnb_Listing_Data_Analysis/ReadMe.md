# Airbnb Listing Data Analysis


## Project Overview

As a consultant working for a real estate start-up, this project involves analyzing Airbnb listing data to investigate the short-term rental market in New York. The goal is to provide insights on private rooms to the real estate company.


## Data Sources

The project uses three data files located in the `data` folder:

- `airbnb_price.csv`: Contains pricing information for various Airbnb listings.
- `airbnb_room_type.xlsx`: Provides details on the types of rooms available for rent.
- `airbnb_last_review.tsv`: Includes information about the last reviews for each listing.

## Objectives

1. Determine the dates of the earliest and most recent reviews and store these values in separate variables.
2. Count the number of listings that are classified as private rooms and store this value in a variable.
3. Calculate the average listing price, rounded to two decimal places, and save this value in a variable.
4. Combine the new variables into a single DataFrame called `review_dates` with the following structure:
   - `first_reviewed`: Date of the earliest review
   - `last_reviewed`: Date of the most recent review
   - `nb_private_rooms`: Number of private room listings
   - `avg_price`: Average listing price
