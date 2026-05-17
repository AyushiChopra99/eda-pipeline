E-Commerce Data Cleaning & EDA Pipeline

Overview
This project performs end-to-end data cleaning and exploratory data analysis
(EDA) on a UK-based online retail dataset containing 500,000+ transactions.
The goal is to uncover customer behavior trends and revenue patterns using Python.


Tools & Technologies
- Python 3
- pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook


Dataset
- Source: Kaggle — E-Commerce Data
- Link: https://www.kaggle.com/datasets/carrie1/ecommerce-data
- Original Rows: 541,909 transactions
- Final Rows (after cleaning): ~397,000
- Columns: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country



Data Cleaning Steps
- Removed 135,080 rows with missing CustomerID values
- Dropped duplicate records (~5,000 rows)
- Removed cancelled orders (InvoiceNo starting with 'C')
- Fixed data types — InvoiceDate converted to datetime, CustomerID to integer
- Added Revenue column (Quantity × UnitPrice)
- Added Month and DayOfWeek columns for time-based analysis



Key Findings
- The United Kingdom accounts for 85%+ of total revenue
- November shows the highest monthly revenue spike — pre-Christmas shopping
- Top product DOTCOM POSTAGE generates the highest single-product revenue
- Thursday is the busiest order day — Sunday has the least activity
- After cleaning, ~145,000 rows were removed to ensure data quality

