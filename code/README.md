# Predicting London House Prices Using Machine Learning

## Project Overview

This project investigates London house prices using historical housing-market data, Consumer Price Index (CPI), Bank Rate and transaction activity.

The main aim is to explore changes in London house prices over time and evaluate different models for predicting monthly borough-level house prices.

The project includes data cleaning, exploratory data analysis, feature engineering, statistical modelling, machine-learning modelling and final model evaluation.

## Project Structure

The analysis is organised into seven Jupyter notebooks and followed in numerical order.

### 01 - Data Cleaning

`01_Data_Cleaning_London_House_Prices.ipynb`

This notebook performs the initial data cleaning and preparation. It checks data types, missing values, duplicates and other data-quality issues before creating the cleaned dataset used in later analysis.

### 02 - Exploratory Data Analysis

`02_EDA_London_Housing.ipynb`

This notebook explores the main patterns in London house prices, transaction activity, CPI and Bank Rate using summary statistics and visualisations.

### 03 - Feature Engineering

`03_Feature_Engineering_London_Housing.ipynb`

This notebook creates features for the predictive models, including

- time-based features;
- seasonal features;
- lagged house-price variables;
- rolling price statistics;
- price-growth variables;
- transaction-related features;
- inflation-related variables.

Lagged and rolling features use historical information to reduce the risk of future-data leakage.

### 04 - Advanced EDA and Borough Inequality

`04_Advanced_EDA_Borough_Inequality.ipynb`

This notebook extends the exploratory analysis by examining differences between London areas. It investigates house-price levels, growth, volatility, transaction activity and price inequality across boroughs.

It also includes comparisons around important market periods such as the 2008 financial crisis.

### 05 - Statistical Modelling and Model Selection

`05_Statistical_Modelling_and_Model_Selection.ipynb`

This notebook examines statistical relationships between the selected variables and London house prices.

It also develops and compares predictive approaches, including Ridge Regression, and includes model diagnostics and time-aware evaluation.

### 06 - Machine Learning and Rolling Backtest

`06_Machine_Learning_and_Rolling_Backtest.ipynb`

This notebook develops a Random Forest regression model and evaluates its forecasting performance using expanding-window yearly backtesting.

The Random Forest is compared with a Seasonal Naive baseline using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE) and R-squared (R²).

### 07 - Final Model Evaluation and Selection

`07_Final_Model_Evaluation_and_Selection.ipynb`

This notebook brings together the final results and compares

1. Seasonal Naive baseline
2. Ridge Regression
3. Random Forest

The models are evaluated using a time-aware framework. MAE is used as the main evaluation metric, with RMSE and R² included as additional measures.

The analysis also examines model consistency, prediction bias, borough-level errors and performance across different borough price levels.

## Dataset Folder

The `Dataset` directory contains the data used and produced during different stages of the project.

```text
Dataset/
├── Original Database/
├── Clean Database/
├── Feature_Engineering_London_Housing/
└── Final Results/
```
