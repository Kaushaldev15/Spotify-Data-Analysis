# Spotify Data Analysis using Python 🎶

This project presents an in-depth exploratory data analysis (EDA) of Spotify track-level data to uncover insights about audio features, song popularity, and music trends. By leveraging Python’s data analysis and visualization libraries, the notebook walks through the end-to-end process of loading, cleaning, transforming, and analyzing Spotify datasets.

---

## 📌 Project Overview

The goal of this project is to analyze Spotify track data to answer questions such as:

* What makes a song popular?
* How do audio features (danceability, energy, tempo, loudness, etc.) correlate with one another?
* Are there clear patterns across genres and release years?
* What insights can we gain about listener preferences?

The project combines **data preprocessing, statistical analysis, and data visualization** to uncover relationships and present findings in an intuitive way.

---

## 🗂 Dataset

The dataset used is `tracks.csv`, which contains detailed metadata for Spotify tracks. Key features include:

* **Track Metadata**: track name, artist(s), release date
* **Popularity Metric**: Spotify’s internal popularity score (0–100)
* **Audio Features**: danceability, energy, loudness, tempo, speechiness, valence, acousticness, instrumentalness, liveness
* **Technical Fields**: duration (in milliseconds), key, mode, explicit flag

---

## ⚙️ Project Workflow

### 1. **Data Import & Exploration**

* Loaded the dataset using **Pandas**.
* Checked for null values, data types, and dataset dimensions.
* Displayed sample records for inspection.

### 2. **Data Cleaning & Preprocessing**

* Converted `release_date` to datetime and set it as the index.
* Converted `duration_ms` to seconds for better interpretability.
* Dropped unnecessary columns such as `key`, `mode`, and `explicit`.
* Handled missing values and normalized fields where required.

### 3. **Exploratory Analysis**

* Identified the **least popular** and **most popular** tracks.
* Conducted descriptive analysis with `df.describe()` to summarize dataset statistics.
* Sampled ~0.4% of data for regression/correlation analysis.

### 4. **Statistical & Correlation Analysis**

* Created **correlation heatmaps** to study relationships among numerical features.
* Analyzed pairwise correlations, e.g.:

  * Loudness vs. Energy
  * Speechiness vs. Popularity
  * Acousticness vs. Danceability

### 5. **Data Visualization**

Generated a wide range of visualizations:

* **Heatmaps** → Feature correlations
* **Histograms** → Popularity distributions
* **Scatterplots** → Track features vs. popularity
* **Regression plots** → Feature relationships (e.g., loudness-energy trends)

### 6. **Insights**

Some key insights derived include:

* **Energy and loudness** show a strong positive correlation.
* Highly popular songs often cluster in certain ranges of **danceability** and **valence**.
* Many unpopular songs share features like high acousticness and low energy.
* Duration trends show how modern tracks are getting shorter over time.

---

## 🛠️ Tech Stack

* **Python**
* **Pandas** – data manipulation
* **NumPy** – numerical operations
* **Matplotlib & Seaborn** – data visualization

---

## 📊 Example Outputs

* **Heatmap of Audio Feature Correlations**
  Visualizes the strength and direction of relationships between features.

* **Regression Plot: Loudness vs Energy**
  Shows strong linear correlation indicating energetic tracks are also louder.

* **Popularity Distributions**
  Highlights imbalance in popularity scores where most songs have lower popularity.

---

## 📘 Project Structure

```
Spotify-Data-Analysis/
│
├── Spotify Data Analysis.ipynb   # Jupyter Notebook with full workflow
├── tracks.csv                    # Dataset (not included in repo due to size)
├── README.md                     # Project documentation
└── requirements.txt              # Python dependencies
```

---

## 🚀 How to Run the Project

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/spotify-data-analysis.git
   cd spotify-data-analysis
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook "Spotify Data Analysis.ipynb"
   ```

4. Run all cells to reproduce the analysis and visualizations.

---

## 🔮 Future Work

* Add **genre-specific analysis** (pop vs. rock vs. hip-hop).
* Build **predictive models** to estimate song popularity.
* Create an **interactive dashboard** (e.g., with Plotly/Dash or Streamlit).
* Expand dataset with more recent Spotify tracks.

---

## 📢 Acknowledgements

* Dataset source: Spotify API / Kaggle.
* Inspired by the power of music data analytics to understand cultural trends.

---

## 👤 Author

**Kaushal Devlekar**

* GitHub: [your profile link]
* LinkedIn: [your LinkedIn link]
* Email: [your email]

---
