# Day-Ahead Electricity Price Forecasting in NO1:
## A Probabilistic Machine Learning Approach for Supporting Large-Scale Consumers in Risk Management

## Overview

This repository contains the work from my Master's thesis in Business Analytics at the University of Inland Norway.

The project focuses on forecasting **day-ahead electricity prices in the Norwegian NO1 bidding area** using statistical and machine learning methods. The objective was to develop accurate forecasting models and provide uncertainty estimates that can support risk management decisions for large-scale electricity consumers.

The study compares a traditional time-series approach (**ARIMA**) with advanced machine learning models (**XGBoost**) and applies explainable AI techniques to understand the key drivers behind electricity price predictions.

---

## Research Objective

The main research question was:

> Can probabilistic machine learning models improve day-ahead electricity price forecasting accuracy and provide useful uncertainty information for risk management?

---

## Business Context

Electricity price volatility creates challenges for large-scale consumers when planning energy costs and managing financial risk.

Accurate price forecasts can support:

- Energy purchasing strategies
- Cost optimization
- Hedging decisions
- Risk management

This project explores how machine learning forecasting can contribute to better decision-making in the Norwegian electricity market.

---

## Data Description

The analysis uses daily observations from the Norwegian **NO1 electricity bidding area** covering the period:

**2015–2025**

The dataset includes:

- Day-ahead electricity prices
- Electricity consumption
- Temperature
- Hydrological reservoir levels
- Natural gas prices (TTF)
- Historical price features and lag variables

Number of observations:

**4,017 daily records**

---

## Methodology

The project follows a time-series forecasting workflow:

### Data Preparation

- Data cleaning
- Feature engineering
- Creation of lag variables
- Time-series train/test split
- Exploratory data analysis

### Forecasting Models

#### ARIMA

A traditional statistical forecasting model used as a benchmark.

#### XGBoost

A machine learning model trained using market, weather, and historical price information.

#### Quantile XGBoost

A probabilistic forecasting approach used to estimate prediction intervals and quantify uncertainty.

---

## Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

### Main Result

The XGBoost model achieved better forecasting performance compared with the ARIMA benchmark.

| Model | MAE (EUR/MWh) |
|---|---:|
| ARIMA | 18.09 |
| XGBoost | 12.30 |

**XGBoost reduced MAE by approximately 32% compared with ARIMA.**

---

## Explainable

To improve model interpretability, SHAP (SHapley Additive exPlanations) analysis was applied.

The analysis identified the most influential variables affecting electricity price predictions, including:

- Previous electricity prices
- Natural gas prices (TTF)
- Market-related variables

---

## Technologies Used

### Programming Languages

- Python

### Python Libraries

- pandas
- NumPy
- scikit-learn
- XGBoost
- Statsmodels
- SHAP
- Matplotlib

### Tools

- Jupyter Notebook
- GitHub

---

## Repository Structure
