# 📊 Forecasting Korean Export Trends Using VAR and Deep Learning

> 📌 A personal project comparing macroeconomic forecasting performance between econometric models and deep learning models.  
> **Type:** Undergraduate research project  
> **Presented at:** CURT (Creative Undergraduate Research Training) 2022  
> **Goal:** Predict Korea's monthly export trends using various economic indicators and compare the reliability of forecasting intervals.

This repository contains a comparative forecasting study between a classical econometric model (VAR) and a deep learning ensemble model using macroeconomic indicators. The objective is to evaluate their short-term predictive performance and confidence interval reliability on export-related time series data.


## 🛠 Features

- VAR (Vector Autoregression) model implementation using `statsmodels`
- Deep learning ensemble model implemented with `PyTorch`
- Sliding window training strategy (5 steps in, 5 steps out)
- Rolling forecast on test set
- Visualization of predicted vs. true export values
- Confidence interval comparison (95% CI)


## 📊 Data Description

| Feature | Description |
|--------|-------------|
| Input | Economic Policy Uncertainty (EPU), Consumer Sentiment Index, Korean Exports |
| Target | Korean Monthly Export Volume |
| Source | Macroeconomic indicators collected from Korean economic data portals |


## 📈 Result Summary

- Deep learning model outperformed VAR in:
  - Lower loss values (smaller RMSE)
  - Narrower 95% confidence intervals
- VAR model showed better performance in very short-term forecasting, but quickly degraded.
- Visual comparison plots (see `/results/`) illustrate predictive behavior and deviation bands.

> ✅ Final Conclusion: **Deep learning model provides more reliable forecasts with tighter uncertainty bounds than classical econometric approaches.**

