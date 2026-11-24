# Week 1: Python, NumPy, pandas, basic ML recap

**Dates:** 23 to 29 Nov · **Time:** 5 h · **Deliverable:** Clean-and-model notebook

**Result:** Titanic survival: Random Forest 84.7% and Logistic Regression 84.4% test accuracy (baseline 61.8%); a tie within noise, so Logistic Regression wins on simplicity.

## Tasks

- [ ] Kaggle Learn Pandas (skim what you know)
- [ ] NumPy quickstart: arrays, shapes, broadcasting, slicing
- [x] Notebook: load a Kaggle tabular dataset, clean it, 3 plots, Random Forest vs Logistic Regression with a train/test split
- [x] Write 3 lines on why one model beat the other

## Notebooks

- [`01_clean_and_model.ipynb`](01_clean_and_model.ipynb)

## Data

Full Titanic passenger list (1,309 passengers) from [OpenML dataset 40945](https://www.openml.org/d/40945), the same data as the Kaggle competition. The notebook downloads it into `data/titanic/titanic.csv` on the first run, so no Kaggle account is needed.
