# 🍫 Chocolate Sales Data
## 📌 Project Overview

This project has the purpose to demonstrate a simple data ETL pipeline using a series of tech stacks, which also acts as a portfolio project.

## 📂 Project Structure
    ├── data/                     # Containing the raw data file
    ├── notebook.ipynb            # Jupyter notebook with pipeline code
    └── README.md                 # This file

## ⚙️ Project Breakdown

### 1. Exploratory Data Analysis (EDA)
- Data cleaning: handling missing/null values, outliers, and data type casting, converting monetary value to float.
- Visualizing temporal, regional and other dimensional sales trends.

### 2. Feature Engineering
- Derived sales success indicator, which is the average box sales value.

### 3. Insights and Recommendations
- The data itself has no stark features to delve deeper into, as the timeframe itself is merely less than a year.
- That exact simplicity makes the data ideal for beginners who just started in diving into the world of data analytics, especially in learning data visualization.

## 🚀 Tech Stack
All the stacks used for this project are python-based compiled in Jupyter Notebook IDE. The python packages used for each specific purpose are as follows:
- **EDA**: pandas, numpy, regex
- **Data Viz**: matplotlib, seaborn

## 📊 Example Outputs
![](../images/python-chocolate_sales_data_top5.png)

![](../images/python-chocolate_sales_data_violin_chart.png)

## 🏗️ How to Run Locally

Clone this repo:

    git clone https://github.com/jasonzelin/data-analytics-portfolio.git
    cd data-analytics-portfolio/chocolate_sales_data


Create virtual environment & install dependencies:

    python -m venv venv
    source venv/bin/activate   # For Linux/Mac OS
    venv\Scripts\activate      # For Windows OS
    pip install -r requirements.txt


Run Jupyter Notebook:

    jupyter notebook


Open **`notebook.ipynb`** and execute cells.

## 🙌 Acknowledgements

- [Atharva Soundankar](https://www.kaggle.com/atharvasoundankar): for providing the datasets in [kaggle](https://www.kaggle.com/datasets/atharvasoundankar/chocolate-sales/data).

- **Open Source Python Packages**: pandas, numpy, re, matplotlib, seaborn