# Google Play Store Analysis

**Track:** Data Analytics (Level 2, Task 4)
**Author:** Syed Mohammed Ghous

## Objective
Perform a comprehensive analysis of the Google Play Store ecosystem — cleaning messy real-world data, exploring app categories, analyzing ratings and pricing trends, and conducting sentiment analysis on user reviews.

## Dataset
Source: [Google Play Store Apps — Kaggle](https://www.kaggle.com/datasets/lava18/google-play-store-apps)

- `googleplaystore.csv` — ~10,800 app listings with category, rating, size, installs, price, and more
- `googleplaystore_user_reviews.csv` — ~64,000 user reviews with pre-labeled sentiment

## What This Notebook Covers
1. **Data Cleaning** — fixed a corrupted row, removed duplicates, handled missing values, converted `Installs`/`Price`/`Size` from text to numeric types
2. **Category Analysis** — most common categories vs. categories with the most installs
3. **Ratings Analysis** — overall rating distribution, average rating by category, free vs. paid comparison
4. **Size vs Installs** — correlation analysis (result: negligible correlation)
5. **Pricing Analysis** — free/paid split, price distribution, estimated revenue by category
6. **Sentiment Analysis** — classified ~37,000 reviews using TextBlob, examined sentiment patterns by category

## Key Insights
1. App count ≠ app popularity — `FAMILY` has the most listed apps, but `GAME` and `COMMUNICATION` dominate total installs.
2. App size has no meaningful correlation with installs (r ≈ 0.13).
3. `GAME` is the most-installed category, but also has the highest negative review sentiment (37%) — high engagement doesn't guarantee high satisfaction.
4. Despite `GAME` leading in installs, `FAMILY` generates the highest estimated paid-app revenue overall.

## Tools Used
Python, pandas, matplotlib, TextBlob, Jupyter Notebook

## Files
- `Google_Play_Store_Analysis.ipynb` — full analysis notebook
- `googleplaystore.csv` / `googleplaystore_user_reviews.csv` — datasets
