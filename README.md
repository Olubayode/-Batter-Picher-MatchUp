# Softball Data Pipeline - XXX Charts API Integration

## 📍 Project Overview

This project automates the retrieval, processing, and organization of ** XXXX Softball Team Data** for the 2024 and 2025 seasons using the **643 Charts API**. The pipeline collects roster data, player-specific hitting and pitching stats (overall and split types), and combines them into **master files** for seamless analysis.

---

## 📂 Folder Structure

```text
ou_softball_project/
├── data/                             # All CSV files stored here
│   ├── ou_roster_2024.csv
│   ├── ou_roster_2025.csv
│   ├── ou_hitting_2024.csv
│   ├── ou_hitting_2025.csv
│   ├── ou_hitting_splits_2024_*.csv  # Each split type saved separately
│   ├── ou_hitting_splits_2025_*.csv
│   ├── ou_pitching_2024.csv
│   ├── ou_pitching_2025.csv
│   ├── ou_pitching_splits_2024_*.csv
│   ├── ou_pitching_splits_2025_*.csv
│   ├── ou_master_hitting_2024.csv    # Final cleaned & merged hitting data
│   ├── ou_master_hitting_2025.csv
│   ├── ou_master_pitching_2024.csv   # Final cleaned & merged pitching data
│   ├── ou_master_pitching_2025.csv
├── config.py                         # Configuration (API URL, Team ID, Season IDs, etc.)



## ⚙️ How It Works

| Step | Action |
|---|---|
| 1️⃣ | Retrieve roster data for each season |
| 2️⃣ | Retrieve overall hitting & pitching stats for each player |
| 3️⃣ | Retrieve split type stats (vs LHP, RHP, home, away) |
| 4️⃣ | Combine all data (overall + splits + roster details) into master files |
| 5️⃣ | Save all data into `data/` folder |

---

## 📥 Data Files Explained

| File Name | What It Contains |
|---|---|
| ou_roster_YYYY.csv | Full roster for the team in that season (names, positions, handedness) |
| ou_hitting_YYYY.csv | Overall season hitting stats (aggregated) |
| ou_hitting_splits_YYYY_{split}.csv | Hitting stats broken down by split (LHP, RHP, Home, Away) |
| ou_pitching_YYYY.csv | Overall season pitching stats (aggregated) |
| ou_pitching_splits_YYYY_{split}.csv | Pitching stats broken down by split (LHH, RHH, Home, Away) |
| ou_master_hitting_YYYY.csv | Combined & cleaned master hitting file (overall + splits + roster data) |
| ou_master_pitching_YYYY.csv | Combined & cleaned master pitching file (overall + splits + roster data) |

---


## ⚙️ How It Works

| Step | Action |
|---|---|
| 1️⃣ | Retrieve roster data for each season |
| 2️⃣ | Retrieve overall hitting & pitching stats for each player |
| 3️⃣ | Retrieve split type stats (vs LHP, RHP, home, away) |
| 4️⃣ | Combine all data (overall + splits + roster details) into master files |
| 5️⃣ | Save all data into `data/` folder |

---

## 📥 Data Files Explained

| File Name | What It Contains |
|---|---|
| ou_roster_YYYY.csv | Full roster for the team in that season (names, positions, handedness) |
| ou_hitting_YYYY.csv | Overall season hitting stats (aggregated) |
| ou_hitting_splits_YYYY_{split}.csv | Hitting stats broken down by split (LHP, RHP, Home, Away) |
| ou_pitching_YYYY.csv | Overall season pitching stats (aggregated) |
| ou_pitching_splits_YYYY_{split}.csv | Pitching stats broken down by split (LHH, RHH, Home, Away) |
| ou_master_hitting_YYYY.csv | Combined & cleaned master hitting file (overall + splits + roster data) |
| ou_master_pitching_YYYY.csv | Combined & cleaned master pitching file (overall + splits + roster data) |

EOF

├── fetch_data.py                     # Fetch data from API and save to CSV
├── process_data.py                   # Process, merge, and clean data into master files
├── main.py                           # Main entry point to run everything
├── README.md                         # This file
