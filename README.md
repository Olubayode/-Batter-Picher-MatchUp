# Softball Data Pipeline - 643 Charts API Integration

## 📍 Project Overview

This project automates the retrieval, processing, and organization of **Oklahoma Softball Team Data** for the 2024 and 2025 seasons using the **643 Charts API**. The pipeline collects roster data, player-specific hitting and pitching stats (overall and split types), and combines them into **master files** for seamless analysis.

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
├── fetch_data.py                     # Fetch data from API and save to CSV
├── process_data.py                   # Process, merge, and clean data into master files
├── main.py                           # Main entry point to run everything
├── README.md                         # This file
