# ⚾ MLB Pitching Data ETL & Velocity Trend Analysis

This project demonstrates a complete end-to-end workflow for extracting, transforming, and analyzing MLB pitch-level data using the `pybaseball` package, with a focus on **Yoshinobu Yamamoto’s** velocity trends.

---

## 📌 Project Overview

The notebook performs the following tasks:

1. **Data Extraction (ETL)**
   - Uses `pybaseball` to retrieve Statcast pitch-by-pitch data
   - Filters and selects relevant columns for pitching analysis
   - Stores raw data into a local PostgreSQL database for scalability and reuse

2. **Data Engineering**
   - Assigns sequential at-bat numbers per pitcher per game
   - Structures the dataset to support longitudinal trend analysis
   - Prepares the dataset for machine learning applications

3. **Exploratory Analysis**
   - Visualizes how Yamamoto’s fastball velocity changes:
     - Over multiple games
     - Across pitch counts (balls/strikes)
     - By at-bat progression within a game
   - Identifies patterns that could indicate fatigue, pacing strategy, or matchup decisions

---

## 🛠️ Tools & Technologies

- **Python** (Pandas, Matplotlib, Seaborn, SQLAlchemy)
- **PostgreSQL** for data storage
- **pybaseball** for Statcast data retrieval
- **Jupyter / Google Colab** for analysis

---

## 📬 Contact

- **Sam Sithimolada**  
[Email Me](mailto:sam.sithimolada.2024@marshall.usc.edu) | [GitHub](https://github.com/ssithimio) | [LinkedIn](https://linkedin.com/in/SamSithimolada)

---

## 🚧 Limitations & Future Work

> Due to the limited 1-week snapshot of collected data, some long-term insights are constrained. With a broader dataset (e.g., full-season tracking), future directions include:
- Pitch usage patterns over time
- Velocity drops as predictors of fatigue or injury risk
- Pitch selection modeling using machine learning
