# Retail Sales EDA

This project presents an academic exploratory data analysis of the supplied Superstore retail transactions. The source dataset is `/Users/atifnawaz/Downloads/Sample - Superstore.csv`; a working copy is stored as `data/retail_sales.csv`.

## Project structure

```text
Retail_Sales_EDA/
├── data/retail_sales.csv
├── notebooks/Retail_Sales_EDA.ipynb
├── outputs/charts/
├── outputs/reports/business_insights.txt
├── requirements.txt
└── README.md
```

## Run the analysis

From this directory, create or activate a Python environment and install dependencies:

```bash
python -m pip install -r requirements.txt
jupyter notebook notebooks/Retail_Sales_EDA.ipynb
```

Run all notebook cells. The notebook reads the real CSV, performs schema-aware cleaning and analysis, displays the figures inline, saves high-resolution PNG charts under `outputs/charts/`, and generates `outputs/reports/business_insights.txt`.

## Dataset limitation

The supplied data contains order, customer, product, sales, quantity, discount, and profit fields. It does not contain customer age or gender, so demographic analysis is explicitly documented as unavailable rather than inferred.
