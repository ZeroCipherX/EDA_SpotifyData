# Spotify EDA: Data-Driven Music Discovery


---

# Spotify Dataset EDA

This project performs an **Exploratory Data Analysis (EDA)** on a Spotify dataset to uncover insights about streaming patterns, artist performance, and audio feature correlations.

---

## Project Structure

* **spotify\_dataset.csv** – Raw dataset used for analysis.
* **spotify\_eda.ipynb** – Jupyter Notebook with step-by-step EDA and visualizations.
* **spotify\_eda.pdf / spotify\_eda.html** – Exported report of the EDA with insights and plots.

---

## Setup & Requirements

To run this project, install the following Python libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

---

## Analysis Steps

1. **Data Loading & Cleaning**

   * Removed unnecessary ID and index columns.
   * Converted numeric-like columns (e.g., Streams, Artist Followers) into numeric types.
   * Handled missing values using mean, mode, and median imputation.
   * Engineered features such as `Release Year`, `Total Chart Presence`, and `Duration (min)`.

2. **Feature Engineering**

   * Created a `Mood Score` using valence and acousticness.
   * Adjusted zero values where invalid by replacing them with medians.

3. **Exploratory Visualizations**

   * Distribution of Streams (log-scaled).
   * Popularity vs. Streams scatterplot.
   * Correlation Heatmap of audio features.
   * Top 10 Artists by Total Streams bar chart.
   * Song Duration Distribution with mean highlighted.
   * Top Genres by Average Streams.
   * Yearly Trends in Average Streams.
   * Outlier detection (Streams & Popularity).

---

## Key Insights

* **Song Duration**: Most tracks are \~3–4 minutes, aligning with commercial standards.
* **Top Artists**: Taylor Swift, BTS, and Justin Bieber dominate total streams.
* **Distribution**: Streaming counts follow a long-tail effect – few mega-hits drive most of the volume.
* **Popularity**: Most songs fall in the 60–90 popularity range, but niche or new tracks can still chart.
* **Audio Features**: High-energy, danceable songs are more likely to achieve streaming success.

---

