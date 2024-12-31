# Movie Data Analysis Project

This project is a comprehensive analysis of a movie dataset, focusing on various attributes such as genres, production companies, spoken languages, and success metrics (popularity, revenue, and ratings). The analysis explores trends in movie success across different categories, providing insights into factors associated with high-performing films.

## Table of Contents

- [Installation](#installation)
- [Project Overview](#project-overview)
- [Data Preprocessing](#data-preprocessing)
- [Analysis and Key Findings](#analysis-and-key-findings)
  - [Genre Analysis](#genre-analysis)
  - [Production Company Analysis](#production-company-analysis)
  - [Language Analysis](#language-analysis)
  - [Adult vs. Non-Adult Films Analysis](#adult-vs-non-adult-films-analysis)
  - [Revenue-to-Budget Ratio Analysis](#revenue-to-budget-ratio-analysis)
- [Visualization Examples](#visualization-examples)
- [License](#license)

## Installation

To set up the environment for this project, follow these steps:

1. Clone the repository.
   ```bash
   git clone https://github.com/Pooria82/Movies-Data-Analysis.git
   cd Movies-Data-Analysis
   ```

2. Install dependencies from the `requirements.txt` file.
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook to see the analysis in detail.
   ```bash
   jupyter notebook Phase1.ipynb
   ```

## Project Overview

The primary goal of this project is to analyze movie data to identify patterns and insights related to movie popularity, success, and genre trends. Through a combination of exploratory data analysis (EDA), feature engineering, and visualizations, this project answers the following questions:

- Which genres are most popular and profitable?
- What are the characteristics of top-performing production companies?
- What languages are most common in successful movies?
- Do adult films perform differently compared to non-adult films?
- Which movies demonstrate high revenue relative to their budget?

## Data Preprocessing

The dataset was cleaned and preprocessed with the following steps:

- **Handling Missing Values**: Replaced missing values in columns like `genres`, `production_companies`, `spoken_languages`, etc.
- **Encoding Categorical Variables**: Used one-hot encoding for multi-label categorical columns like `genres` and `production_companies`.
- **Feature Engineering**: Created new features such as:
  - `ROI` (Revenue-to-Budget Ratio)
  - `success_metric` (a custom score based on popularity, vote count, and revenue)
  - `genre_similarity_score` and `content_complexity` (to measure similarity and complexity of genres for each movie)

## Analysis and Key Findings

### Genre Analysis

Using the `genres` column, we identified popular genres based on the number of films, average rating, and average revenue. This analysis provides insights into which genres are more likely to receive higher ratings and generate more revenue, giving an indication of audience preferences.

### Production Company Analysis

This analysis focuses on identifying production companies that have produced the most high-rating films. Additionally, it examines if these films are successful in terms of popularity, revenue, and rating. For instance, major companies like **Walt Disney Productions** and **Warner Bros. Animation** show trends of higher average revenue.

### Language Analysis

The `spoken_languages` column was analyzed to determine the distribution of languages used in movies and their success. English is the most common language, but films in other languages like Japanese and French also appear to have considerable representation.

### Adult vs. Non-Adult Films Analysis

The `adult` column was used to separate adult-oriented films and assess if these movies achieve higher ratings, popularity, or revenue. The results provide insight into whether adult films perform differently in terms of success metrics.

### Revenue-to-Budget Ratio Analysis

Using the `revenue` and `budget` columns, we calculated the Revenue-to-Budget Ratio (ROI) to identify movies that were financially successful. High-ROI movies are considered financially successful, demonstrating strong returns relative to their budget.

## Visualization Examples

The project includes several visualizations created using `matplotlib` and `seaborn`:

- **Genre Distribution**: Visualizes the most common genres and their average ratings and revenue.
- **Top Production Companies**: Shows the count of high-rating movies produced by top companies and their average popularity, rating, and revenue.
- **Language Distribution**: Pie chart displaying the distribution of spoken languages across movies.
- **Adult vs. Non-Adult Film Comparison**: Compares the success metrics of adult vs. non-adult films.

Each visualization provides a deeper understanding of the trends and patterns within the movie dataset.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this code, as long as you include the original copyright and license notice in any substantial portions of the software.