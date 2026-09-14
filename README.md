# Cross-Country Spending Analysis

## Project Overview

This project analyzes spending patterns across two different geographic markets during comparable periods.

The goal is to build an end-to-end data analytics workflow, transforming raw financial transaction data into structured, reliable, and actionable insights.

The project covers the complete analytics process, from data extraction and cleaning to SQL analysis, data modeling, and dashboard development.

---

## Business Question

> How do spending patterns differ between two geographic markets during comparable periods?

The analysis will explore:

- Total spending
- Monthly spending trends
- Number of transactions
- Average transaction value
- Spending by category
- Essential vs. discretionary spending
- Recurring vs. one-off expenses
- Differences between comparable periods

---

## Project Workflow

```text
Raw Documents
      ↓
Data Extraction
      ↓
CSV / Raw Data
      ↓
Python + pandas
      ↓
Data Cleaning & Transformation
      ↓
SQL Server
      ↓
Data Modeling
      ↓
Analytical SQL
      ↓
Power BI
      ↓
Insights & Recommendations
```

---

## Tools

- Python
- pandas
- SQL Server
- Power BI
- Power Query
- DAX
- Git & GitHub

---

## Data Architecture

The project will use a layered approach.

### Raw Data

Original transaction data before transformation.

### Staging Layer

Intermediate data used for cleaning, validation, standardization, and transformation.

### Analytical Model

The final dataset will be structured using a star schema.

Planned model:

```text
                 dim_date
                    |
                    |
dim_category — fact_transaction — dim_account
                    |
                    |
                dim_market
```

The grain of the fact table is:

> One row represents one financial transaction.

---

## Repository Structure

```text
cross-country-spending-analysis/
│
├── data/
│   ├── raw/
│   │   ├── pdf/
│   │   └── csv/
│   ├── processed/
│   └── sample/
│
├── notebooks/
│   └── 01_pdf_to_csv.ipynb
│
├── src/
│   ├── extract.py
│   ├── transform.py
│   └── load.py
│
├── sql/
│   ├── staging/
│   ├── dimensions/
│   ├── fact/
│   └── analysis/
│
├── powerbi/
│
├── docs/
│
├── .gitignore
├── requirements.txt
└── README.md
```

---

## Data Privacy

The original dataset is not included in this repository.

Sensitive information and raw financial documents are kept outside version control.

Any data made publicly available in this repository will be anonymized or replaced with sample data to protect privacy.

---

## Planned Analysis

The project will investigate questions such as:

1. How does total spending differ between the two markets?
2. Which spending categories account for the largest share of expenses?
3. How does average transaction value differ?
4. Are spending patterns stable across comparable months?
5. Which categories explain the largest differences between markets?
6. How much spending is recurring, essential, discretionary, or exceptional?

---

## Project Status

🚧 **Work in progress**

Current stage:

**Data extraction and preparation**

Next steps:

- Extract transaction data
- Create the raw dataset
- Clean and standardize transactions
- Perform data quality checks
- Build the SQL staging layer
- Design the star schema
- Perform exploratory and analytical SQL analysis
- Build DAX measures
- Develop the Power BI dashboard
- Document insights and conclusions

---

## Skills Demonstrated

This project is designed to demonstrate practical skills in:

- Data extraction
- Data cleaning
- Data quality
- Python and pandas
- ETL concepts
- SQL
- Analytical SQL
- Data modeling
- Star schema design
- Power Query
- DAX
- Power BI
- Data visualization
- Business analysis
- Data storytelling
