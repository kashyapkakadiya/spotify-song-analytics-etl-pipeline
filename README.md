# Spotify Song Analytics ETL Pipeline

## Overview
This project demonstrates a complete **ETL (Extract, Transform, Load) pipeline** for music streaming data using the “Most Streamed Spotify Songs 2024” dataset. It showcases core data engineering skills—data cleaning, transformation, database loading, and analytics—targeted for entry-level data engineer roles.

## Stack
- **Python:** pandas, sqlite3
- **Google Colab:** development environment
- **SQLite:** local database for analytics

## Steps

### 1. Extract
- Loaded CSV music data into a pandas DataFrame in Google Colab.

### 2. Transform
- Converted columns with numeric stats (e.g., streams, playlist counts) to proper types.
- Fixed date formats and standardized fields.
- Handled missing values—dropped where essential, filled with zero elsewhere.

### 3. Load
- Exported the cleaned DataFrame to a SQLite database table.
- Enabled SQL queries for insights.

### 4. Analytics
- Top streamed songs and artists.
- Trends by release year.
- Additional analysis via SQL queries.

***

## Pipeline Architecture

```mermaid
flowchart LR
    A[Raw CSV file] --> B[Extract with pandas]
    B --> C[Transform (Clean & Standardize)]
    C --> D[Load to SQLite DB]
    D --> E[SQL Analytics & Insights]
```
