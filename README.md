# Netflix Movies and TV Shows Data Analysis Using SQL

![Netflix Logo](https://github.com/Vanshika2899/netflix_sql_project/blob/main/BrandAssets_Logos_02-NSymbol.jpg)

## Overview

This project analyzes the Netflix Movies and TV Shows dataset using PostgreSQL. The goal is to perform exploratory data analysis (EDA) and solve real-world business problems using SQL queries.

The dataset was sourced from Kaggle and contains information about Netflix content, including movies, TV shows, directors, cast members, countries, ratings, genres, release years, and descriptions.

---

## Project Objectives

* Explore Netflix content trends.
* Compare Movies and TV Shows distribution.
* Analyze content ratings and genres.
* Identify top-producing countries.
* Discover popular actors and directors.
* Categorize content based on description keywords.
* Practice advanced SQL concepts such as:

  * Common Table Expressions (CTEs)
  * Window Functions
  * Aggregate Functions
  * String Manipulation
  * Date Functions
  * Data Cleaning

---

## Dataset

Source: Netflix Movies and TV Shows Dataset from Kaggle

Dataset contains the following attributes:

| Column Name  | Description                  |
| ------------ | ---------------------------- |
| show_id      | Unique identifier            |
| type         | Movie or TV Show             |
| title        | Title of content             |
| director     | Director name                |
| casts        | Cast members                 |
| country      | Country of production        |
| date_added   | Date added to Netflix        |
| release_year | Year of release              |
| rating       | Content rating               |
| duration     | Movie duration or TV seasons |
| listed_in    | Genre/category               |
| description  | Content description          |

---

## Database Schema

```sql
CREATE TABLE netflix
(
    show_id VARCHAR(6),
    type VARCHAR(10),
    title VARCHAR(150),
    director VARCHAR(208),
    casts VARCHAR(1000),
    country VARCHAR(150),
    date_added VARCHAR(50),
    release_year INT,
    rating VARCHAR(10),
    duration VARCHAR(15),
    listed_in VARCHAR(100),
    description VARCHAR(250)
);
```

---

## Technologies Used

* PostgreSQL
* SQL
* Kaggle Dataset
* pgAdmin

---

## Business Problems Solved

### 1. Count the Number of Movies vs TV Shows

Determine the distribution of content types available on Netflix.

### 2. Find the Most Common Rating for Movies and TV Shows

Identify the dominant audience rating category for each content type.

### 3. List Movies Released in 2020

Filter movies released during a specific year.

### 4. Top 5 Countries with the Most Netflix Content

Analyze which countries contribute the most content.

### 5. Find the Longest Movie

Identify the movie with the maximum duration.

### 6. Find Content Added in the Last 5 Years

Track recently added Netflix content.

### 7. Find All Movies/TV Shows by Rajiv Chilaka

Filter content by a specific director.

### 8. List TV Shows with More Than 5 Seasons

Identify long-running television series.

### 9. Count Content Items in Each Genre

Analyze genre distribution across Netflix.

### 10. Average Content Released by India Per Year

Evaluate content contribution trends from India.

### 11. Find Documentary Movies

Filter content categorized as documentaries.

### 12. Find Content Without a Director

Identify missing director information.

### 13. Movies Featuring Salman Khan in the Last 10 Years

Analyze actor-specific appearances.

### 14. Top 10 Actors Appearing in Indian Content

Determine the most frequently featured actors in Indian productions.

### 15. Content Categorization Using Keywords

Classify content as:

* Bad Content → contains keywords "kill" or "violence"
* Good Content → all other content

---

## SQL Concepts Demonstrated

* GROUP BY
* ORDER BY
* LIMIT
* Aggregate Functions
* Window Functions (RANK)
* Common Table Expressions (CTE)
* String Functions
* Date Functions
* CASE Statements
* Subqueries
* Data Filtering
* Data Transformation

---

## Key Insights

* Movies constitute a larger share of Netflix content than TV Shows.
* The United States and India are among the largest content contributors.
* Documentary content represents a significant portion of the catalog.
* Netflix content additions increased significantly in recent years.
* Certain actors and directors appear frequently across multiple titles.

---

## Project Structure

```
Netflix-SQL-Analysis
│
├── Dataset
│   └── netflix_titles.csv
│
├── SQL Queries
│   └── netflix_analysis.sql
│
├── Screenshots
│   └── query_results.png
│
├── README.md
│
└── schema.sql
```

---

## How to Run

1. Create a PostgreSQL database.
2. Create the netflix table using the schema provided.
3. Import the Kaggle dataset.
4. Execute the SQL queries.
5. Analyze the results.

---

## Learning Outcomes

This project strengthened my understanding of:

* Relational Databases
* Data Analysis using SQL
* PostgreSQL Functions
* Business Problem Solving
* Query Optimization
* Data Cleaning and Transformation

---

## Author

Vanshika

LinkedIn: [linkedin profile](https://www.linkedin.com/in/vanshika-singhal-93a857171/)

---

## License

This project is created for educational and portfolio purposes.

