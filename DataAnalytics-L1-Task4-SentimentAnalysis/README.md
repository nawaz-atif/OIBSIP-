# Task 4: Sentiment Analysis Using NLP and Machine Learning

This project analyzes the supplied Amazon Fine Food Reviews dataset with NLTK text preprocessing, TF-IDF features, Multinomial Naive Bayes, Logistic Regression, evaluation charts, WordClouds, and real error analysis.

## Dataset

The notebook uses the original dataset at `/Users/atifnawaz/Downloads/Reviews.csv`. The 287 MB source is intentionally not duplicated in Git because GitHub rejects files larger than 100 MB. No data is fabricated or replaced.

The dataset contains five review scores. The notebook maps the documented ordinal scale to three sentiment classes: scores 1-2 become `Negative`, score 3 becomes `Neutral`, and scores 4-5 become `Positive`. This is a transparent rating-based mapping, not an invented third class.

## Project structure

```text
DataAnalytics-L1-Task4-SentimentAnalysis/
├── notebooks/Sentiment_Analysis_NLP.ipynb
├── outputs/charts/
├── requirements.txt
└── README.md
```

## Run

From this project directory:

```bash
python -m pip install -r requirements.txt
jupyter notebook notebooks/Sentiment_Analysis_NLP.ipynb
```

The notebook loads the real CSV, removes exact review duplicates, preprocesses review text while preserving negation, fits TF-IDF only on training data, trains two classifiers on the same stratified split, creates metrics/confusion matrices/WordClouds, displays five real errors, and reports a final checklist.
