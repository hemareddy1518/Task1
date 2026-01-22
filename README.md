# Task1
Understanding Dataset &amp; Data Types

A short, step-by-step guide for exploring datasets and preparing them for machine learning. Focuses on data types, missing values, statistical summaries, and identifying features and targets.

## Table of Contents
- Overview
- Dataset(s) Included
- Repository Structure
- Prerequisites
- How to Use
- EDA Checklist / Key Steps
- Learning Outcomes
  
## Overview
Step-by-step analysis of datasets to prepare for ML tasks. The exercises demonstrate basic exploratory data analysis (EDA) techniques and how to evaluate dataset suitability for regression/classification problems.

## Datasets Included
- Students Performance Dataset — Predict math scores (regression). (https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)

## Repository Structure
- README.md — this file
- StudentsPerformance.csv — expected directory for CSV datasets
- Data_Analysis.ipynb — Jupyter notebooks with EDA examples
- Dataset_Analysis_Report.pdf — report

## Prerequisites
- Python 3.8+
- pandas, numpy, matplotlib, seaborn

Install required packages:

```bash
pip install pandas numpy matplotlib seaborn
```

## How to Use
1. Load the dataset CSV file.
2. Open the notebook or run the example script:

```python
import pandas as pd

df = pd.read_csv("students_performance.csv")
df.head()
```

3. Follow the EDA checklist below to inspect and clean the data.

## EDA Checklist / Key Steps
- Import libraries (pandas, numpy, matplotlib/seaborn)
- Load dataset and inspect rows: `head()`, `tail()`
- Check dataset shape: `df.shape`
- Inspect schema and missing values: `df.info()` and `df.isnull().sum()`
- Get statistical summary: `df.describe()`
- Identify column types: numerical, categorical, binary, ordinal
- Explore unique values in categorical columns: `df['col'].value_counts()`
- Detect and handle missing values or incorrect types
- Define target variable and input features
- Assess dataset suitability for ML (enough samples, class balance, missingness)

## Learning Outcomes
- Understand dataset structure and data types
- Detect and handle missing and categorical data
- Prepare datasets for ML models (classification/regression)
- Gain confidence in basic EDA techniques
