# Titanic Survival Prediction

This project focuses on building a machine learning pipeline to predict passenger survival on the Titanic. It involves extensive data preprocessing, feature engineering, and binary classification using the classic Titanic dataset.

## 🚀 Project Overview

The goal is to analyze passenger data (such as age, gender, and boarding port) to determine the factors that most influenced survival rates and to train a model that can predict outcomes for new data.

## 🛠️ Data Preprocessing & Engineering

Key steps taken in the data cleaning process include:
* **Missing Value Imputation:** * Filled missing `Age` values using the median to maintain distribution.
    * Handled missing `Embarked` values using the mode (most frequent port).
* **Categorical Encoding:**
    * **Sex:** Converted to binary integers (male: 0, female: 1).
    * **Embarked:** Transformed using One-Hot Encoding (`pd.get_dummies`) with `drop_first=True` to avoid the dummy variable trap.
* **Feature Selection:** Separated features ($X$) from the target variable ($y$ - Survived) to prepare for model training.

## 📂 Project Structure

```text
titanic-survival-prediction/
├── data/
│   ├── train.csv          # Training dataset
│   └── test.csv           # Test dataset
├── .venv/                 # Python virtual environment
├── main.ipynb             # Main analysis and modeling notebook
└── README.md              # Project documentation
