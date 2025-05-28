# ETL Pipeline: From API to CSV with Python

This project demonstrates a simple but powerful ETL (Extract, Transform, Load) process using only Python. It connects to a public API, processes the data, and stores it in a structured CSV file for further analysis.

---

## 🚀 Project Overview

- **Language:** Python
- **Objective:** Automate data extraction from an API, clean/transform the data, and save it as a CSV file.
- **Use Case:** You can adapt this pipeline to monitor cryptocurrency prices, weather conditions, news headlines, or any structured API data.

---

## 🧰 Tech Stack

- `requests`: For API consumption
- `pandas`: For data cleaning and transformation
- `datetime`: For handling time formats
- `os`: For file system operations


---

## 🔄 ETL Process Breakdown

### 1. Extract
Connects to a public REST API (e.g. OpenWeatherMap, CoinGecko) and retrieves JSON data.

### 2. Transform
Processes the raw data:
- Renames columns
- Parses dates and timestamps
- Handles missing values
- Filters or aggregates where needed

### 3. Load
Saves the cleaned data into a `data/output.csv` file.

---

## 🛠️ How to Run the Project

### 1. Clone the repo
```bash
git clone https://github.com/SCifu88/ETL_from_API_to_CSV.git
cd api-to-csv-etl
```

### 2. Create a virtual environment
``` bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

### 3. Install dependencies
``` bash
pip install -r requirements.txt
```

### 4. Run the pipeline
``` bash
python src/etl_pipeline.py
```

