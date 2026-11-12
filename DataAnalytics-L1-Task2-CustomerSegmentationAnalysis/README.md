# OIBSIP Data Analytics Level 1 Task 2: Customer Segmentation Analysis

This project completes OIBSIP Data Analytics Level 1, Task 2: Customer Segmentation Analysis. It uses RFM features and K-Means clustering on the supplied Online Retail transaction workbook. The original source file remains unchanged at `/Users/atifnawaz/Downloads/Online Retail.xlsx`.

The source dataset is `/Users/atifnawaz/Downloads/Online Retail.xlsx`; a working copy is stored as `data/Online Retail.xlsx`.

## Project structure

```text
DataAnalytics-L1-Task2-CustomerSegmentationAnalysis/
├── data/Online Retail.xlsx
├── notebooks/Customer_Segmentation_Analysis.ipynb
├── outputs/charts/
├── outputs/reports/business_insights.txt
├── requirements.txt
└── README.md
```

## Run the analysis

From this directory, create or activate a Python environment and install dependencies:

```bash
python -m pip install -r requirements.txt
jupyter notebook notebooks/Customer_Segmentation_Analysis.ipynb
```

Run all notebook cells. The notebook reads the supplied Excel workbook, performs schema-aware cleaning, builds customer-level RFM features, standardises them, evaluates K from 1 to 10 with the elbow method, fits K-Means with a fixed random state, displays the figures inline, and generates the included PNG charts and `outputs/reports/business_insights.txt`.

The notebook preserves the original workbook and uses a working copy in memory for cleaning.

## Dataset limitation

The supplied data contains transaction, product, date, price, customer, and country fields. It does not contain customer age or gender, so demographic analysis is explicitly unavailable rather than inferred. RFM monetary value and CLV are based on observed completed transaction revenue; they are not forecasts.
