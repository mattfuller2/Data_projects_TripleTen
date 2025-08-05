# 🎬Sprint 1: IMDb Ratings

This repository contains the code and analysis for the project "Show Rating Analysis," which aims to analyze the relationship between show ratings and the number of votes. The project uses a dataset containing information about shows, their ratings, genres, and release years.

## Project Overview

The primary objective of this project is to explore the correlation between show ratings and the number of votes they received, as well as identifying patterns within the dataset related to duplicates, missing values, and outliers. The dataset includes a wide range of shows, from movies to TV series, and spans several genres.

## Project Structure

- **Data Cleaning:**
  - Handling missing values in the dataset.
  - Changing data types for specific columns where necessary (e.g., `release_year` or `imdb_score`).
  - Removing duplicates to ensure data integrity.
  
- **Data Analysis:**
  - Exploring the distribution of show ratings and the number of votes.
  - Investigating patterns between highly-rated shows and the volume of votes received.
  
- **Conclusions:**
  - The analysis shows that highly-rated shows, particularly those released during what is considered the "Golden Age" of television, tend to have more votes.
  - Shows with mid-range ratings (scores of 7-9) are most popular in terms of vote count.

## Installation

To run the code in this repository, you need to have the following dependencies installed:

- Python 3.x
- Jupyter Notebook
- pandas
- numpy
- matplotlib (if visualizations are used)

You can install the required packages using the following command:

```bash
pip install -r requirements.txt
