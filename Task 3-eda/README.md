# Task 3 - Netflix EDA (Exploratory Data Analysis)

## Problem Statement
Analyze Netflix's content library to identify trends and patterns.

## 📊 Dataset
- **Source:** [Netflix Movies and TV Shows (Kaggle)](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- **File:** netflix_titles.csv
- **Size:** 8,807 entries, 12 columns

## 🧹 Data Cleaning
- Filled missing `director`, `cast`, and `country` values with "Not Stated"
- Dropped 17 rows with missing `rating`, `duration`, or `date_added`
- Converted `date_added` to datetime format
- Extracted `year_added` and `month_added` as new columns
- Confirmed no duplicate rows

## 🔑 Key Insights
1. **Content Type:** Movies make up ~70% of Netflix's library (6,126) vs TV Shows (~30%, 2,664)

2. **Top Producing Countries:** The United States leads with 2,809 titles, followed by India (972) — reflecting strong Bollywood presence on the platform

3. **Growth Trend:** Content addtions grew steadily from 2016-2019, peaking in 2019 during Netflix's agressive global expansion. Additions declined after 2019, likely due to the disruptions of COVID-19 and a strategic shift toward quality over quantity

## 🔨 Tools Used
- Python, Pandas, Matplotlib, Seaborn
- Jupyter Notebook (VS Code)

## 📂 Files
- `netflix_eda.ipynb` — Full analysis notebook
- `netflix_titles.csv` — Raw dataset
- `netflix_cleaned.csv` — Cleaned dataset