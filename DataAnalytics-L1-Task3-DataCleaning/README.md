# Task 3: Professional Data Cleaning and Preprocessing

This project cleans the supplied cafe sales dataset for a university data-quality assignment. The original source is `/Users/atifnawaz/Downloads/dirty_cafe_sales.csv`; an unchanged working copy is stored in `data/dirty_cafe_sales.csv`.

## Project structure

```text
DataAnalytics-L1-Task3-DataCleaning/
├── data/dirty_cafe_sales.csv
├── notebooks/Data_Cleaning_Preprocessing.ipynb
├── output/charts/
├── output/cleaned_dataset.csv
├── requirements.txt
└── README.md
```

## Run

From this directory:

```bash
python -m pip install -r requirements.txt
jupyter notebook notebooks/Data_Cleaning_Preprocessing.ipynb
```

The notebook inspects the actual CSV, reports quality problems before cleaning, documents column-specific treatments, detects IQR outliers without deleting legitimate values, saves a new cleaned CSV, reloads it, and verifies the result. The original dataset is never overwritten.
