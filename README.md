# Student Withdrawal Prediction Using Machine Learning

A comparative study of k-Nearest Neighbours and Logistic Regression for predicting university student withdrawal.

## Overview

This project analyses student demographic, academic, and institutional data to predict withdrawal risk using supervised learning. Two algorithms are compared to identify at-risk students early in their academic journey.

## Dataset

**Source:** UCI Machine Learning Repository - "Predict Students' Dropout and Academic Success"
- 4,424 students from Portuguese higher education
- 36 features covering demographics, academics, and institutional factors
- Binary classification: withdrawal vs. continuation

## Models Compared

- **k-Nearest Neighbours (k-NN):** Instance-based learning with distance metrics
- **Logistic Regression:** Linear probabilistic classification with regularisation

## Key Features

- Comprehensive exploratory data analysis (EDA)
- Data leakage prevention (2nd semester features removed)
- Feature engineering for high-cardinality variables
- Multicollinearity assessment and mitigation
- Hyperparameter tuning with cross-validation
- Threshold analysis for optimal performance

## Requirements

- Python 3.11.5
- Dependencies listed in `requirements.txt`

## Installation

```bash
pip install -r requirements.txt
```

## Usage

1. **Run EDA:** `eda_full.py` - Complete dataset analysis
2. **Train k-NN:** `k-NN_full.py` - k-NN model with grid search
3. **Train Logistic:** `logistic_regression_full.py` - Logistic regression with regularisation

Configuration managed via `config.toml`.

## Results

| Model | Accuracy | Withdrawal Recall | Precision |
|-------|----------|-------------------|-----------|
| k-NN | 81.5% | 63.0% | 75.2% |
| Logistic Regression | 81.0% | 74.3% | 69.0% |

## Project Structure

```
├── eda_full.py              # Exploratory data analysis
├── k-NN_full.py             # k-NN implementation
├── logistic_regression_full.py # Logistic regression implementation
├── config.toml              # Configuration file
├── requirements.txt         # Python dependencies
├── datasets/                # Data directory
└── README.md               # This file
```

## Author

Craig Moore - MSc AI Module HEP502 Assignment