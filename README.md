# Project Overview

This dissertation investigates how different feature spaces and dimensionality reduction techniques influence the forecasting performance of Long Short-Term Memory (LSTM) models in the context of stock market prediction.

The study designs and implements a modular software system to support experimentation with two distinct feature spaces:
- A **simple feature space** based solely on historical price data.
- A **complex feature space** enriched with technical indicators and macroeconomic variables.

Dimensionality reduction was explored through two key techniques:
- **Recursive Feature Elimination (RFE)**
- **Principal Component Analysis (PCA)**

By applying these methods, the research aims to optimize the input space for the LSTM models, reducing redundancy and improving generalization.

Models were trained to perform **single-step forecasts** of daily closing prices. Their performance was evaluated using:
- **Statistical error metrics**: Mean Absolute Percentage Error (MAPE) and Root Mean Squared Error (RMSE).
- A **simulated trading strategy** to assess practical effectiveness.

The results provide insights into the comparative strengths of different feature engineering approaches and dimensionality reduction methods, highlighting the trade-offs between model complexity, accuracy, and real-world applicability. This combined evaluation underscores the importance of thoughtful data preprocessing and feature optimization in building robust financial forecasting models.

---

# Models Trained

A total of **18 models** were trained for this research:

## 1. Data Length Analysis
- **6 models** (3 for the S&P 500 and 3 for the FTSE 100)
- Each group trained with different historical data lengths: **20 years**, **10 years**, and **5 years**.
- **Goal**: Investigate how the amount of historical data impacts LSTM forecasting performance.

## 2. PCA-Optimized Feature Space
- **6 models** (3 for the S&P 500 and 3 for the FTSE 100)
- Each group trained on datasets reduced with PCA, retaining **95%**, **97%**, and **99%** of the original variance.
- **Goal**: Evaluate how dimensionality reduction via PCA affects model performance.

## 3. RFE-Optimized Feature Space
- **6 models** (3 for the S&P 500 and 3 for the FTSE 100)
- Each group trained on datasets optimized using RFE, selecting **13**, **10**, and **7** key features.
- **Goal**: Assess how recursive feature selection impacts forecasting accuracy.

---
