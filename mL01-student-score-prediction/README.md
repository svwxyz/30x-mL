# Student Score Prediction

A simple machine learning project that predicts a student's exam score based on **hours studied** and **attendance** using Linear Regression.

## What's in the project

```
mL-student-score-prediction/
├── data/student_data.csv    # 50 students, 3 columns
├── model.ipynb              # Notebook with the full workflow
└── README.md
```

**Dataset columns:** `hours_studied`, `attendance`, `exam_score` (the target).

## What the notebook does

1. Loads the CSV with pandas.
2. Checks the data (`head`, `info`, missing values).
3. Plots hours studied vs exam score with seaborn.
4. Selects `hours_studied` and `attendance` as features.
5. Splits the data 70/30 into train and test sets.
6. Trains a `LinearRegression` model.
7. Predicts test scores and compares them with actual scores.
8. Evaluates using R², MSE, and MAE.

## Result

| Metric | Value |
| --- | --- |
| R² Score | 0.994 |
| MSE | 2.55 |
| MAE | 1.12 |

The model fits the data very well — predictions are off by about 1.1 points on average.

## How to run

```bash
pip install pandas seaborn scikit-learn jupyter
jupyter notebook model.ipynb
```

## Author

**Sumit Vishwakarma** — completed on **November 5, 2026**
