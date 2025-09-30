# 🗽 NYC Taxi ETL Pipeline
## 📌 Project Overview

This project has the purpose to demonstrate a simple data ETL pipeline using a series of tech stacks, which also acts as a portfolio project.

## 📂 Project Structure
    ├── data/                     # Containing the raw and transformed data files
    ├── notebook.ipynb            # Jupyter notebook with pipeline code
    ├── requirements.txt          # Python dependencies
    └── README.md                 # This file

## ⚙️ ETL Pipeline Steps

### 1. Extract
- Source: [NYC Taxi Trips dataset](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page).
- Downloaded parquet files.

### 2. Transform
- Cleaned missing/null values
- Ensured typecasting accordingly.
- Mapped pickup/dropoff location IDs using lookup tables.
- Example transformations: concatenation, joins, enums.

### 3. Load
- Transformed data written to:
    - Local Parquet/CSV (zero-cost version).
    - BigQuery table (if GCP console billing-enabled).

## 🚀 Tech Stack

- Python (Pandas for data exploration and API libraries for PySpark and BigQuery)

- PySpark (scalable transformations, joins, mapping, schema handling)

- Google BigQuery (data warehouse)

- Google Cloud Service Account for authentication

<!-- ## 📊 Example Outputs

Show a few sample rows (e.g., vendor mapping, pickup/dropoff zones). 

Include screenshots (like .png) of transformations or schema. -->

## 🏗️ How to Run Locally

Clone this repo:

    git clone https://github.com/jasonzelin/data-analytics-portfolio.git
    cd data-analytics-portfolio/new_york_taxi_trips


Create virtual environment & install dependencies:

    python -m venv venv
    source venv/bin/activate   # For Linux/Mac OS
    venv\Scripts\activate      # For Windows OS
    pip install -r requirements.txt


Run Jupyter Notebook:

    jupyter notebook


Open **`nyc_taxi_etl.ipynb`** and execute cells.

## 🔑 Credentials & Config

For BigQuery:

Place your service account JSON key locally.

Set environment variable:

    export GOOGLE_APPLICATION_CREDENTIALS="/path/to/service_account.json"


If running without BigQuery (zero-cost mode), pipeline still runs end-to-end with local files.

## 📈 Future Improvements

- Automate ETL with Apache Airflow / Cloud Composer. (*Requires cost*)

- Add streaming ingestion with Kafka or Pub/Sub. (*Requires cost*)

- Deploy on GCP Dataproc for distributed processing. (*Requires cost*)

- Unit tests for transformations.

## 🙌 Acknowledgements

- **NYC Taxi & Limousine Commission**: for providing open datasets.

- **Google Cloud**: for BigQuery/PySpark tools.