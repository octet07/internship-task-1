# Titanic Data Analysis

This notebook performs basic data analysis on the Titanic dataset, including data loading, cleaning, feature engineering, scaling, and visualization.

## Table of Contents

1. [Setup and Data Loading](#1-setup-and-data-loading)  
2. [Basic Data Exploration](#2-basic-data-exploration)  
3. [Handling Missing Values](#3-handling-missing-values)  
4. [Encoding Categorical Features](#4-encoding-categorical-features)  
5. [Scaling Numerical Features](#5-scaling-numerical-features)  
6. [Data Visualization and Outlier Removal](#6-data-visualization-and-outlier-removal)

---

## 1. Setup and Data Loading

- The necessary libraries are imported: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn.preprocessing`, etc.
- The Titanic dataset is loaded from Google Drive (or a local path, as per implementation).
- Initial inspection is done using functions like `head()`, `info()`, and `describe()`.

---

## 2. Basic Data Exploration

- Summary statistics and structure of the dataset are explored.
- The number of missing values per column is computed.
- Types of each column and their distributions are analyzed.

---

## 3. Handling Missing Values

- **Age**: Missing values are filled using the **mean** or **median**.
- **Embarked**: Missing values are filled using the **mode**.
- **Cabin**: This column is dropped due to a high percentage of missing data.
- **Fare**: Rows with missing fare values are removed from the dataset.

---

## 4. Encoding Categorical Features

- **Sex** and **Embarked** columns are encoded using **Label Encoding** from `sklearn.preprocessing`.
- This converts categorical values into numerical format suitable for machine learning models.

---

## 5. Scaling Numerical Features

- Features like `Age`, `Fare`, `Pclass`, `SibSp`, and `Parch` are scaled using **StandardScaler**.
- Standardization improves model performance by bringing all features to a similar scale.

---

## 6. Data Visualization and Outlier Removal

- **Boxplots** are generated using `seaborn` to visualize distribution and spot outliers.
- Outliers in the **Fare** column are detected and removed using the **Interquartile Range (IQR)** method.

---

> ✅ This data preprocessing and cleaning step prepares the Titanic dataset for further analysis or machine learning model development.
