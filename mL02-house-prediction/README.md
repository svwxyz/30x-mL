# House Price Prediction

A simple machine learning project that predicts house prices based on **area, bedrooms, bathrooms, and floors** using Linear Regression.

## What's in the project

```
mL02-house-prediction/
├── data/house_prices.csv    # 105 houses, 6 columns
├── main.ipynb               # Notebook with the full workflow
└── README.md
```

**Dataset columns:** `Area`, `Bedrooms`, `Bathrooms`, `Floors`, `Age`, `Price` (the target).

## What the notebook does

1. Loads the CSV with pandas.
2. Checks the data (`head`, `shape`, `info`, `describe`, missing values).
3. Explores the data with histograms, boxplots, scatter plots, and a correlation heatmap.
4. Selects `Area`, `Bedrooms`, `Bathrooms`, and `Floors` as features.
5. Splits the data 70/30 into train and test sets.
6. Trains a `LinearRegression` model.
7. Predicts test prices and compares them with actual prices.
8. Evaluates using R², MAE, and MSE.

## Result

| Metric | Value |
| --- | --- |
| R² Score | 0.988 |
| MAE | 262,108 |
| MSE | 1.23 × 10¹¹ |

The model fits the data very well — predictions are off by about 2.6 lakh on average.

## How to run

```bash
pip install pandas seaborn matplotlib scikit-learn jupyter
jupyter notebook main.ipynb
```

## Author

**Sumit Vishwakarma** — completed on **November 5, 2026**
