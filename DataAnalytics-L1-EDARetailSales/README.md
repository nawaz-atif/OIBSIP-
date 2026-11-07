# Retail Sales EDA

This project is a university-level exploratory data analysis of a retail sales CSV using pandas, NumPy, Matplotlib, and Seaborn.

## Dataset

This project uses the supplied `Sample - Superstore.csv` dataset. The original CSV remains unmodified in the project root.

```text
```

The notebook loads the source with `latin1` encoding and does not fabricate records or assume fixed column names. It detects common variants of date, sales/revenue, quantity, profit, product, category, age, gender, and customer ID columns, and documents unavailable analyses when fields are absent.

## Run

```bash
cd DataAnalytics-L1-EDARetailSales
python -m pip install -r requirements.txt
jupyter notebook notebooks/Retail_Sales_EDA.ipynb
```

Run all cells from top to bottom. Generated PNG charts are saved to `outputs/charts/`, and the calculated narrative report is saved to `outputs/reports/business_insights.txt`.

## Structure

- `Sample - Superstore.csv`: original input dataset
- `notebooks/Retail_Sales_EDA.ipynb`: executable analysis
- `outputs/charts/`: high-resolution figures
- `outputs/reports/`: business insights report
- `requirements.txt`: Python dependencies
