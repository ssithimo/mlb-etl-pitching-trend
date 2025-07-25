# ⚾ MLB Pitching Data ELT & Velocity Trend Analysis

This project builds a complete ELT pipeline to collect, store, and analyze MLB pitch-level data using the `pybaseball` library. Data is ingested into a PostgreSQL database and analyzed using Python, with a case study focused on Yoshinobu Yamamoto’s pitch velocity trends.

Due to limited capacity, only a weeks worth of data was loaded. 07/01/2025 - 07/07/2025

---

## 🔧 Tech Stack

- **Languages:** Python, SQL
- **Libraries:** pybaseball, pandas, SQLAlchemy, matplotlib, seaborn, dotenv
- **Database:** PostgreSQL (local)
- **Automation:** Cron (for scheduled updates)

---

## 🚀 Features

✅ ELT Pipeline for Pitching Data
- Extracts pitch-by-pitch MLB data using pybaseball
- Selects 30+ relevant features for pitching analysis
- Loads cleaned data into a PostgreSQL database using SQLAlchemy
- Enables flexible querying and analysis with minimal latency

📊 Yoshinobu Yamamoto Case Study
- Filters dataset to analyze Yamamoto’s outings
- Tracks average fastball velocity by:
  - Game date
  - At-bat number
  - Count and pitch number
- Engineers a new pitch_at_bat_number field to sequentially number batters he faced

⏰ Scheduled Updates
- Supports automated weekly ELT using cron

---

## 📋 Questions Explored

1. How does Yamamoto's average velocity trend over the game per inning?
2. Does Yamamoto's pitch velocity decrease as at-bat count increases?
3. Are Yamamoto's fastballs slower in high-pitch counts?
4. How does Yamamoto's pitching velocity differ over counts?
5. How does Yamamoto's average velocity trend over the game at different at-bats?
6. How does Yamamoto's pitch velocity trend over games?

---

## 🔮 Future Improvements
- Add cloud storage integration (e.g., Supabase, AWS RDS)
- Build ML models to predict next pitch type using game context
- Visualize pitch maps and spin data for deeper scouting reports

---

📬 Contact
Sam Sithimolada
📧 [Email](mailto:sam.sithimolada.2024@marshall.usc.edu)
🔗 [LinkedIn](linkedin.com/in/SamSithimolada)
[GitHub](https://github.com/ssithimio)

