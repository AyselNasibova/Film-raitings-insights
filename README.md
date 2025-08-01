
# 🎬 IMDb Films Analysis with Python

A data-driven exploratory analysis of popular films using IMDb data. This project utilizes Python (Pandas, Seaborn, Matplotlib) in a Jupyter Notebook environment to uncover trends, insights, and visualizations from a movie dataset.

## 📌 Project Overview

This notebook explores a film dataset with a focus on:
- Genre distribution
- Release year trends
- IMDb rating patterns
- Duration analysis
- Most frequent directors
- Country-wise production counts

By visualizing and cleaning the data, this project helps understand what defines popular films and how certain features (like genre or country) affect film production and ratings.

---

## 📊 Key Features

- 🔍 Data Cleaning & Preprocessing  
- 📈 Rating Distributions Visualization  
- 🎞️ Genre and Duration Correlation  
- 🧠 Top Directors and Most Used Languages  
- 🌍 Country-level Production Analysis  
- 📆 Release Year Histogram  
- 🎯 Insightful bar charts, countplots, pie charts, and more  

---

## 📁 Project Structure

```
films-analysis/
├── films_analiz.ipynb          # Jupyter Notebook with full EDA
├── dataset/                    # (Optional) Folder for CSV file
│   └── imdb_top_films.csv      # Original or processed dataset
├── images/                     # Saved visualizations
│   ├── rating_distribution.png
│   ├── genre_bar_chart.png
│   └── release_year_trend.png
├── README.md                   # Project documentation (this file)
└── requirements.txt            # Python packages used
```

---

## 🛠️ Libraries Used

- `pandas`
- `matplotlib`
- `seaborn`

Install dependencies with:

```bash
pip install -r requirements.txt
```

---

## 📸 Sample Visualizations

> ![Rating Distribution](images/rating_distribution.png)
> *IMDb Rating Distribution*

> ![Genre Breakdown](images/genre_bar_chart.png)
> *Top Genres by Frequency*

---

## 📂 Dataset Source

The dataset used in this project is based on top-rated IMDb films (can be replaced with other IMDb CSV sources or Kaggle datasets).

---

## 📌 Insights & Takeaways

- The most frequent film genres are **Drama**, **Comedy**, and **Action**.
- IMDb ratings show a bell-curve pattern centered around 7.
- Film production peaked in the late 1990s and early 2000s.
- The USA dominates movie production, followed by India and the UK.

---

## 📈 Author

This project was developed for educational and portfolio purposes. Feel free to fork or contribute!
