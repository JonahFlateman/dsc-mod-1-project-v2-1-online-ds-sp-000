# Module 1 Final Project readme

In this project, we will do a data analysis to see which movies are currently doing the best at the box office and see what insights can be gleaned for our client looking to produce new movies.  Below we will list our goals and methodologies for the project.

## Datasets

For this project we will be using datasets provided to us by The Numbers ('tn.movie_budgets.csv.gz') and IMDB ('imdb.title.basics.csv.gz' and 'imdb.title.ratings.csv.gz').

## Goals

* Learn which types of movies earn the most revenue
* Use return on investment (ROI) as a key metric and compare with production budget and release year
* Compare success of different genres and further explore a specific genre's ROI, production budget, and worldwide gross
* Examine user ratings compared to ROI for trends and outliers

## Methodologies

### Importing and Cleaning

* Import datasets as listed above as DataFrames
* Convert any necessary string columns to integer columns
* Remove dollar signs and commas from necessary integer columns
* Check for duplicates and NaN values

### Merging

* Drop columns that will not be used in final DataFrame
* Change all title columns to "movie" prior to merging on this column
* Create "ROI" column to sort by (worldwide gross minus production budget)
* Remove duplicates using a groupby (taking only first instance of a movie's title), then removing NaN values
* Slice "release date" to year only and converting to integer

### Analysis and Visualizations

* Analyze our ROI compared with movie title, year, and production budget using several visualizations
* Further analyze our successful genre ROIs and study data and more successful movies in a specific genre
* Look at user rating as a possible metric of success and identify the role of outlier data points