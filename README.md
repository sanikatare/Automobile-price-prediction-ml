# Car Price Prediction using Machine Learning

## Overview

This project implements an end-to-end machine learning pipeline for automobile price prediction using the Car Features and MSRP dataset. The objective is to analyze vehicle specifications, identify the factors affecting car prices, and build predictive models capable of estimating MSRP values based on technical and market-related attributes.

The project covers the complete machine learning workflow including:

* Data preprocessing
* Exploratory data analysis
* Feature engineering
* Outlier handling
* Regression modeling
* Model evaluation
* Data visualization

The implementation was developed in Python using industry-standard data science and machine learning libraries.

---

# Problem Statement

Car pricing depends on multiple variables such as engine specifications, transmission type, fuel efficiency, brand value, and vehicle category. Predicting vehicle prices accurately is a common real-world regression problem in the automotive and e-commerce domains.

The goal of this project is to:

* Analyze automobile pricing patterns
* Identify the most influential pricing factors
* Build machine learning models for MSRP prediction
* Evaluate regression performance using standard metrics
* Develop a clean and reproducible ML workflow

---

# Dataset

## Source

Car Features and MSRP Dataset
https://www.kaggle.com/datasets/CooperUnion/cardataset

## Dataset Description

The dataset contains technical specifications and pricing information for various car models.

### Features Include

| Feature           | Description             |
| ----------------- | ----------------------- |
| Make              | Manufacturer name       |
| Model             | Vehicle model           |
| Year              | Manufacturing year      |
| Engine HP         | Horsepower              |
| Engine Cylinders  | Number of cylinders     |
| Transmission Type | Transmission category   |
| Vehicle Style     | Body style              |
| Highway MPG       | Highway fuel efficiency |
| City MPG          | City fuel efficiency    |
| Popularity        | Market popularity score |
| MSRP              | Target variable         |

---

# Project Workflow

## 1. Data Preprocessing

The dataset was cleaned and prepared before model training.

### Steps Performed

* Removed duplicate records
* Handled missing values
* Dropped irrelevant columns
* Checked data consistency
* Converted categorical variables
* Standardized numerical features

### Libraries Used

```python id="1m8czq"
import pandas as pd
import numpy as np
```

---

## 2. Exploratory Data Analysis

Exploratory analysis was conducted to understand feature distributions and relationships.

### Analysis Performed

* Distribution analysis
* Correlation analysis
* Outlier analysis
* Feature relationship analysis
* MSRP trend analysis

### Visualizations Used

* Heatmaps
* Histograms
* Boxplots
* Scatterplots
* Distribution plots

### Key Observations

* Engine horsepower showed strong correlation with MSRP.
* Luxury vehicle brands had significantly higher pricing distributions.
* MSRP contained extreme outliers.
* Fuel efficiency and vehicle category affected pricing trends.

---

# Feature Engineering

Feature engineering was applied to improve model performance.

### Techniques Used

* Label Encoding
* Feature Selection
* Correlation Filtering
* Outlier Treatment

### Encoding Example

```python id="3cl8af"
from sklearn.preprocessing import LabelEncoder
```

---

# Outlier Handling

Outliers were identified using the Interquartile Range (IQR) method and visual inspection through boxplots.

### Methods Applied

* Outlier detection
* Outlier removal/capping
* Distribution normalization

Handling outliers improved regression stability and reduced skewness in pricing data.

---

# Machine Learning Models

The project focuses primarily on regression modeling for MSRP prediction.

## Models Implemented

### Linear Regression

Used as a baseline regression model for performance comparison.

### Decision Tree Regressor

Implemented to capture nonlinear feature relationships.

### Random Forest Regressor

Used for improved predictive performance through ensemble learning.

---

# Model Evaluation

Model performance was evaluated using standard regression metrics.

| Metric   | Purpose                           |
| -------- | --------------------------------- |
| MAE      | Measures average prediction error |
| MSE      | Penalizes larger errors           |
| RMSE     | Root error magnitude              |
| R² Score | Measures explained variance       |

### Example

```python id="7y14x4"
from sklearn.metrics import mean_absolute_error
from sklearn.metrics import mean_squared_error
from sklearn.metrics import r2_score
```

---

# Technologies Used

| Technology       | Purpose                     |
| ---------------- | --------------------------- |
| Python           | Core programming language   |
| Pandas           | Data preprocessing          |
| NumPy            | Numerical computation       |
| Matplotlib       | Data visualization          |
| Seaborn          | Statistical visualization   |
| Scikit-learn     | Machine learning            |
| Jupyter Notebook | Experimentation environment |

---

# Repository Structure

```text id="v9f7e6"
car-price-prediction-ml/
│
├── ML.ipynb
├── README.md
├── requirements.txt
├── .gitignore
├── dataset/
│   └── automobile_data.csv
├── images/
└── outputs/
```

---

# Installation

## Clone Repository

```bash id="ykgv9o"
git clone https://github.com/yourusername/car-price-prediction-ml.git
```

## Navigate to Project Directory

```bash id="ydjxt2"
cd car-price-prediction-ml
```

## Install Dependencies

```bash id="vz1m4p"
pip install -r requirements.txt
```

## Launch Notebook

```bash id="f2vt7k"
jupyter notebook
```

---

# Requirements

```text id="mwg0ph"
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

# Results

The project successfully demonstrates:

* End-to-end machine learning workflow implementation
* Real-world data preprocessing
* Effective exploratory data analysis
* Regression model development
* Feature impact analysis on car pricing
* Visualization-driven insights

The pipeline produces reliable predictive performance for automobile price estimation tasks.

---

# Future Improvements

Potential enhancements include:

* Hyperparameter tuning
* Cross-validation
* XGBoost implementation
* Feature scaling optimization
* Model deployment using Flask or Streamlit
* Interactive dashboard integration

---

# Skills Demonstrated

This project demonstrates practical experience in:

* Machine Learning
* Regression Analysis
* Data Cleaning
* Feature Engineering
* Exploratory Data Analysis
* Data Visualization
* Model Evaluation
* Python Development

---


# Conclusion

This project demonstrates a structured machine learning workflow for automobile price prediction using real-world vehicle data. It combines preprocessing, exploratory analysis, feature engineering, regression modeling, and evaluation into a reproducible pipeline suitable for learning, experimentation, and portfolio demonstration.
