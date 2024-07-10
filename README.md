
# Fandango Movie Ratings Analysis

## Overview

This project investigates whether Fandango is artificially boosting movie ratings, potentially due to their interest in selling more tickets. I compare Fandango's displayed scores with review ratings from other sites and normalize all ratings to a 0 to 5 star range for consistency.

## Project Breakdown

### Part 1: Data Collection and Initial Exploration

In this section, we focus on collecting and exploring the data needed to answer our main question about Fandango's rating practices.

1. **Data Collection**:
    - Collected data from various sources including Fandango, Rotten Tomatoes, Metacritic, and IMDB.
    - Ensured that the datasets included consistent columns for fair comparison.

2. **Initial Exploration**:
    - Conducted a basic exploratory data analysis to understand the structure of our data.
    - Identified key columns and ensured all necessary data points were included.

### Part 2: Data Cleaning and Preparation

In part two, we delve into cleaning and preparing our data for analysis. This is crucial for ensuring accurate results.

1. **Data Cleaning**:
    - Removed any null values and ensured all ratings were properly formatted.
    - Addressed inconsistencies in movie titles across different datasets.

2. **Data Preparation**:
    - Normalized ratings from all sources to a uniform 0 to 5 star scale.
    - Prepared a combined dataset for detailed analysis.

### Part 3: Analysis and Findings

To the final part of the Project. Here, we answer the key question: Is Fandango artificially boosting ratings?

1. **Combining Data**:
    - Merged Fandango's data with other review sites' data using an inner join on the movie titles.
    - Ensured that only movies present in both datasets were included to avoid null values.

2. **Normalization**:
    - Converted all ratings to a 0 to 5 scale for fair comparison.
    - Used simple division for normalization (e.g., dividing by 20 for 0-100 scales, by 2 for 0-10 scales).

3. **Analysis**:
    - Created a normalized scores dataframe for easier plotting and comparison.
    - Used various plotting techniques to compare distributions of ratings:
        - KDE plots to visualize the density of ratings.
        - Histograms to show the distribution of ratings across different sites.

4. **Findings**:
    - Fandango's ratings were consistently higher than those from other sites.
    - Fandango displayed ratings much higher than the true numeric ratings, especially for lower-rated movies.
    - Official critics from Rotten Tomatoes and other sites rated movies more harshly compared to Fandango's ratings.


### Conclusion

This project clearly demonstrates that Fandango's displayed ratings are significantly higher than those from other review platforms. Whether this is due to an intentional bias or user preferences on Fandango is unclear, but the data shows a notable discrepancy.

### Project Files

- **Jupyter Notebook**: Contains all code for data collection, cleaning, normalization, and analysis.
- **Data Files**: CSV files from Fandango, Rotten Tomatoes, Metacritic, and IMDB.

---

### References

- [Wikipedia Article on Fandango](https://en.wikipedia.org/wiki/Fandango_(company))
- [538 Article on Fandango Ratings](https://fivethirtyeight.com/features/fandango-movies-ratings/)

---


This README file summarizes the project's key points, guiding any reader through the process and findings of the analysis.