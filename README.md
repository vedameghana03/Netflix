# Netflix

# Netflix Data Analysis

This project involves performing data analysis on a Netflix dataset using Python and the pandas library.

## Dataset

The dataset used is `Netflix+Dataset.csv`. It contains information about movies and TV shows available on Netflix, including details such as show ID, category, title, director, cast, country, release date, rating, duration, type, and description.

## Project Goals

The primary goals of this project are to analyze the Netflix dataset using pandas. Specific operations include:

1.  Detecting and removing duplicate records.
   
2.  Identifying and visualizing null values using a heatmap.
   
3.  Answering specific questions about the dataset, such as:
    * Finding the Show ID and director for the show "House of Cards."
    * Determining the year with the highest number of TV show and movie releases.
    * Counting the number of movies and TV shows.
    * Listing movies released in the year 2000.
    * Listing titles of TV shows released only in India.
    * Identifying the top 10 directors with the most TV shows and movies.
    * Filtering records based on category, type, or country.
    * Finding how many movies/shows Tom Cruise was cast in.
    * Analyzing different ratings.
    * Finding the maximum duration of a movie/show.

## Libraries Used

* pandas
* seaborn
* matplotlib.pyplot

## Code Description

1.  **Import pandas:** The pandas library is imported for data manipulation and analysis. [cite: 119]
   
2.  **Load the dataset:** The dataset is loaded into a pandas DataFrame. [cite: 119]
   
3.  **Data Exploration:**
   * The code displays the first few rows of the dataset. [cite: 121, 122]
   * The code determines the shape (number of rows and columns) and size of the dataset. [cite: 122]
   * The code retrieves the column names and their data types. [cite: 122, 123]
   * The code provides a concise summary of the dataset, including column names, data types, non-null counts, and memory usage. [cite: 123]
4.  **Duplicate Record Handling:**
   * The code checks for duplicate records in the dataset. [cite: 124, 126]
   * The code removes duplicate records from the dataset. [cite: 126, 128, 129, 131]
5.  **Null Value Analysis:**
   * The code calculates the number of null values in each column. [cite: 131, 132]
   * A heatmap is generated to visualize the distribution of null values. [cite: 132]
6.  **Data Analysis and Filtering:**
   * The code filters the dataset to find records related to "House of Cards". [cite: 134, 135]
   * The code converts the 'Release Date' column to datetime format for further analysis. [cite: 136, 137, 140]
   * The code determines the count of releases per year and visualizes it using a bar chart. [cite: 141]
   * The code counts the occurrences of each category ('Movie' and 'TV Show') and visualizes it using a countplot. [cite: 142, 144, 145]
   * The code filters the dataset to display movies released in the year 2000. [cite: 75, 77, 105]
   * The code filters the dataset to show TV show titles released in India. [cite: 78]
   * The code identifies the top 10 directors based on the number of releases. [cite: 118, 121]
   * The code filters records based on specified conditions for 'Category', 'Type', and 'Country'. [cite: 127, 150, 80, 81, 82, 83]
   * The code determines how many movies/shows Tom Cruise was cast in. [cite: 152, 153, 154, 155, 156, 84, 85, 86, 87, 88, 89]
   * The code analyzes the different ratings present in the dataset. [cite: 90, 91, 92, 93, 94]
   * The code finds the maximum duration from the `Duration` column. [cite: 95, 96, 97]

## Results

* Duplicate records were identified and removed. [cite: 126, 128, 129, 131]
   
* Null values were visualized using a heatmap. [cite: 132]
   
* Analysis was performed to answer questions related to:
    * "House of Cards" details. [cite: 134, 135]
    * Release year analysis. [cite: 141]
    * Category counts. [cite: 142, 144, 145]
    * Movie releases in 2000. [cite: 75, 77, 105]
    * TV shows released in India. [cite: 78]
    * Top 10 directors. [cite: 118, 121]
    * Filtering by category, type, and country. [cite: 127, 150, 80, 81, 82, 83]
    * Tom Cruise cast appearances. [cite: 152, 153, 154, 155, 156, 84, 85, 86, 87, 88, 89]
    * Rating analysis. [cite: 90, 91, 92, 93, 94]
    * Maximum duration. [cite: 95, 96, 97]

## Code Snippets

### Load Dataset

```python
import pandas as pd
data = pd.read_csv("Netflix+Dataset.csv")
