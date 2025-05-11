# Netflix Movies and TV Shows Analysis using SQL
![netflix logo](wp12900350-4k-netflix-wallpapers.png)

This project involves a comprehensive analysis of Netflix's movies and TV shows data using SQL. The goal is to extract valuable insights and answer various business questions to understand content distribution, ratings, geographical trends, and more.

## 📌 Overview

The analysis includes:
- Distribution of content types (movies vs TV shows)
- Most common ratings for movies and TV shows
- Content analysis by release years, countries, and durations
- Content categorization based on specific criteria and keywords
- Geographical distribution of content
- Director and actor analysis

## 🗃️ Dataset

The data for this project is sourced from Kaggle:

[Netflix Movies and TV Shows Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)

### Database Schema

```sql
CREATE TABLE netflix (
    show_id VARCHAR(5),
    type VARCHAR(10),
    title VARCHAR(250),
    director VARCHAR(550),
    casts VARCHAR(1050),
    country VARCHAR(550),
    date_added VARCHAR(55),
    release_year INT,
    rating VARCHAR(15),
    duration VARCHAR(15),
    listed_in VARCHAR(250),
    description VARCHAR(550)
);
```

## Business Problems and SQL Solutions

### 1. Content Type Distribution

```sql
    SELECT type, COUNT(*) 
    FROM netflix 
    GROUP BY 1;
```



