# Project: Global Cinema Trends & Box Office Performance
## Movie Dataset Exploratory Data Analysis (EDA) with Python :chart_with_upwards_trend: :bar_chart:

This project performs a step-by-step Exploratory Data Analysis (EDA) on a real-world movie dataset using Python. The analysis covers data exploration, cleaning, and visualization to uncover patterns in genres, ratings, and box office trends.


## Tech Stack

1. Language: Python - Pandas, Matplotlib, Seaborn, Numpy
2. Notebook Environment: Jupyter Notebook


## Dataset Source

Kaggle: [URL](https://www.kaggle.com/datasets/mjshubham21/movie-dataset-for-analytics-and-visualization)

## Dataset Overview

A quick overview of the dataset on Kaggle, detailing the columns such as movie ID, title, genre, release year, budget, box office numbers, IMDb rating, Rotten Tomatoes score, director, and lead actor
## Exploratory Data Analysis

### 1. Data Loading & Initial Inspection

* Loading the CSV file into a pandas DataFrame
* Viewing DataFrame information (.info()) to understand data types and memory usage
* Displaying the first and last rows of the DataFrame using .head() and .tail()
* Retrieving row and column counts using .shape
* Accessing column-wise data types (.dtypes)

### 2. Descriptive Statistics 

* Generating descriptive statistics for numerical columns using .describe()
* Focusing on IMDb rating and Rotten Tomatoes score for average and standard deviation

### 3. Missing and Duplicate Values

* Checking for missing values using .isna().sum()
* Checking for duplicated rows using .duplicated().sum()

### 4. Histograms for Numerical Distributions 

* Identifying numerical columns for plotting
* Generating histograms using seaborn.histplot to visualize distributions of budget, box office, IMDb rating, and Rotten Tomatoes score
* Analysis of distributions (e.g., more movies with lower budgets, higher ratings having more movies)

### 5. Bar Plots for Categorical Distributions

* Identifying categorical columns
* Creating bar plots using value_counts().head(20).plot(kind='bar') for top 20 genre, country, director, and lead actor counts
* Discussion on the most frequent categories (e.g., Drama as the clear winner in genres, USA in countries)

### 6. Relationship Analysis (Scatter Plots)

* **Budget vs. Global Box Office:** Plotting budget against global box office using seaborn.scatterplot with logarithmic scales to observe their correlation
* **IMDb vs. Rotten Tomatoes Ratings:** Plotting IMDb rating against Rotten Tomatoes score to analyze their relationship, noting instances where ratings diverge

### 7. Group By Analysis

* **Average Ratings & Revenues by Genre and Release Year:** Grouping data by genre and release year to calculate average global box office, budget, IMDb rating, and Rotten Tomatoes score
* **Line Plot of Average Global Box Office by Genre Over Years:** Visualizing trends in average global box office for different genres over time
* Filtering by specific genres (e.g., Action) to see their individual trends

### 8. Top Actors by Average IMDb Rating

* Grouping data by lead actor and calculating their average IMDb rating
* Sorting values to find the top actors with the highest average ratings and visualizing them with a bar plot


## Screenshots

| Average Global Genres | Genre Counts | IMDb Ratings |
| :---: | :---: | :---: |
| <img src="https://github.com/amandebnath/movie-analysis/blob/main/Screenshots/avg_global_genres.png" alt="avg_global_genres" width="200" height="200"> | <img src="https://github.com/amandebnath/movie-analysis/blob/main/Screenshots/genre_counts.png" alt="genres_counts" width="200" height="200"> | <img src="https://github.com/amandebnath/movie-analysis/blob/main/Screenshots/imdb_ratings.png" alt="imdb_ratings" width="200" height="200"> |
