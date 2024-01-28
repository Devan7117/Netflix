# Netflix Prize Dataset Recommendation System

This project implements a Recommendation System for the Netflix Prize Dataset using Singular Value Decomposition (SVD). The dataset includes customer ratings for various movies, and the goal is to predict and recommend movies to users based on their preferences.

## Dataset

- The main dataset is loaded from the 'combined_data_1.txt' file, containing customer IDs, movie ratings, and other information.
- The 'movie_titles.csv' file is used to get additional details about movies.

## Requirements

- Python 3.x
- pandas
- matplotlib
- scikit-surprise

Install the required packages using the following command:

```bash
pip install pandas matplotlib scikit-surprise
```

# Overview

**Data Loading and Preprocessing:**

Reads the main dataset file and additional movie titles file.
Converts the 'Rating' column to a float and handles missing values.

**Data Cleaning:**

Filters out movies and customers with fewer reviews (top 30% rated movies and active users).
Creates a ratings matrix for further analysis.

**Singular Value Decomposition (SVD):**

Uses the Surprise library to perform SVD for collaborative filtering.
Computes the Root Mean Squared Error (RMSE) of the SVD algorithm.

**User-Specific Recommendations:**

Provides movie recommendations for a specific user (e.g., user with ID 712664).
Utilizes SVD predictions to suggest top-rated movies for the user.

# Notes

- This project is part of the Netflix Prize Dataset, and it demonstrates collaborative filtering using SVD for movie recommendations.

- The dataset contains customer ratings, and the system predicts and suggests top-rated movies for a specific user.

- The SVD algorithm is implemented using the Surprise library, and its performance is evaluated based on RMSE.
