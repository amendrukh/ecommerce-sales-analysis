# E-commerce Performance Dashboard

This project explores the performance of an e-commerce business using **SQL**, **Python**, and **Tableau**. It covers the full analytics workflow: extracting data from a database, exploring and analyzing it in Python, and building an interactive dashboard for business users.

The project was created as part of my Data Analytics portfolio.

## Project Goals

The project focuses on three main areas:

- extracting and combining data from Google BigQuery using SQL;
- exploring the dataset and performing statistical analysis in Python;
- creating an interactive Tableau dashboard to monitor key business metrics.

## Project Structure

```
ecommerce-sales-analysis/
│
├── notebooks/
│   └── E_commerce_analysis.ipynb
│
├── tableau/
│   └── E-commerce_Performance_Dashboard.twbx
│
├── images/
│   ├── dashboard 1.png
│   └── dashboard 2.png
│
└── README.md
```

## Dataset

The dataset was built by joining multiple tables from the Google BigQuery Data Analytics dataset.

Each record contains information about:

- order date
- session ID
- continent and country
- device, browser and operating system
- device model
- browser language
- traffic source and traffic channel
- registered user information
- email verification status
- newsletter subscription status
- product category
- product name
- product price
- product description

### Dataset Assumption

This dataset assumes that **one order contains exactly one product**.

Because of that:

- **Revenue** is calculated as the sum of product prices (`SUM(Price)`).
- **Orders** are calculated as the number of purchased products.
- Each row represents a single purchased item.

---

## Data Analysis

The Python notebook includes:

- data extraction from Google BigQuery;
- dataset overview and data quality checks;
- missing value analysis;
- exploratory data analysis (EDA);
- sales performance analysis;
- customer behavior analysis;
- traffic source analysis;
- device and operating system analysis;
- pivot tables;
- correlation analysis;
- statistical hypothesis testing;
- additional business insights and visualizations.

The analysis answers questions such as:

- Which continents and countries generate the highest sales?
- Which product categories perform best?
- How do sales vary across devices and traffic channels?
- How do registered and non-registered users differ?
- Does newsletter subscription affect purchasing behavior?
- Are there statistically significant relationships between key business metrics?

## Tableau Dashboard

The Tableau dashboard provides an interactive overview of the main e-commerce KPIs.

It includes:

- Total Revenue
- Total Orders
- Total Sessions
- Average Order Value (AOV)
- Conversion Rate
- Previous Period comparison
- Revenue trend
- Sales distribution by weekday
- Dynamic metric selection
- Custom date range comparison
- Interactive filters for:
  - Country
  - Continent
  - Device
  - Operating System
  - Category
  - Traffic Channel

### Interactive Dashboard

https://public.tableau.com/app/profile/anna.mendrukh/viz/Book134444/Dashboard1?publish=yes

## Python Notebook

Google Colab notebook:

https://colab.research.google.com/drive/15WN5GFkP060nk8WaGCifwD7k0TRJRX27?usp=sharing

## Technologies

- SQL (Google BigQuery)
- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Tableau Public

## Repository Contents

- SQL data extraction
- Python data analysis
- Statistical analysis
- Tableau dashboard
- Project documentation
