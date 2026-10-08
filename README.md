revise this:
<div align="center">

# 🌸 Byte & Bloom Analytics
### *E-Commerce Data Pipeline, SQL Modeling & Interactive Dashboard*

[![Python](https://img.shields.io/badge/Python-FFB6C1?style=for-the-badge&logo=python&logoColor=333333)](#)
[![SQL](https://img.shields.io/badge/SQL-FFD1DC?style=for-the-badge&logo=postgresql&logoColor=333333)](#)
[![Pandas](https://img.shields.io/badge/Pandas-FF69B4?style=for-the-badge&logo=pandas&logoColor=white)](#)
[![Jupyter](https://img.shields.io/badge/Jupyter-FFC0CB?style=for-the-badge&logo=jupyter&logoColor=333333)](#)
[![Streamlit App](https://img.shields.io/badge/Streamlit-FFB6C1?style=for-the-badge&logo=streamlit&logoColor=333333)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-E0BBE4?style=for-the-badge)](#)

*Building clean data pipelines, relational schemas, and dynamic visual dashboards from 100k+ Brazilian e-commerce transactions.*

</div>

---

## 💅🏽 Overview
This repository bridges backend software engineering and analytical storytelling using the [Olist Brazilian E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce). 

Rather than running an exploratory script inside a single giant notebook, this project treats data analysis like a structured software engineering workflow:
1. **Data Wrangling & Pipeline:** Processing raw CSVs, fixing datetimes, and joining tables cleanly using Python and Pandas.
2. **Relational Database & SQL:** Loading processed data into SQLite to run queries on customer lifetime value, fulfillment delays, and category margins.
3. **Interactive Dashboard:** Wrapping the dataset inside a dynamic Streamlit web application so anyone can interact with the findings live.

---

## 🛠️ Tech Stack & Tools
* **Language & Environment:** Python 3.12 | Jupyter Notebook
* **Data Wrangling:** Pandas, NumPy
* **Database & Querying:** SQLite | Relational Schema Design & Window Functions
* **Dashboard & UI:** Streamlit
* **Data Visualization:** Seaborn, Matplotlib (Styled with custom pastel themes)

---

## 💡 Key Business Questions Explored

* **Shipping Latency vs. Customer Satisfaction:** How many days of delivery delay does it take before review scores drop sharply?
* **Payment Behavior:** How do installment options influence order basket sizes across budget vs. premium items?
* **Category Profitability:** Which product categories bring in top revenue versus which ones incur high fulfillment costs and delays?

---

## 📂 Repository Structure
```text
byte-and-bloom-analytics/
├── data/                   
├── notebooks/
│   ├── 01_data_cleaning.ipynb  
│   └── 02_eda_visuals.ipynb   
├── sql/
│   ├── schema_setup.sql         
│   └── business_queries.sql    
├── app.py                       
├── requirements.txt             
├── .gitignore
├── LICENSE
└── README.md
```

---

## 🚀 How to Run Locally

### 1. Clone the Repository & Set Up Environment
```bash
git clone [https://github.com/fatemasadik07/byte-and-bloom-analytics.git](https://github.com/fatemasadik07/byte-and-bloom-analytics.git)
cd byte-and-bloom-analytics

# Create and activate a virtual environment
python -m venv .venv
.venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### 2. Download the Dataset
1. Download the [Olist E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) from Kaggle.
2. Unzip and place all `.csv` files inside the `data/` directory.

### 3. Run the Data Pipeline & Analysis
Launch Jupyter Notebook to execute the ETL pipeline and visualizations:
```bash
jupyter notebook
```
Open `notebooks/01_data_cleaning.ipynb` and run all cells to clean and generate processed tables in `data/`.

### 4. Launch the Interactive Dashboard
Run the Streamlit web application locally:
```bash
streamlit run app.py
```
