This dissertation investigates how different feature spaces and dimensionality reduction techniques influence the forecasting performance of Long Short-Term Memory (LSTM) models in the context of stock market prediction. The study designs and implements a modular software system to support experimentation with two distinct feature spaces: a simple space based solely on historical price data, and a complex space enriched with technical indicators and macroeconomic variables.
Dimensionality reduction was explored through two key techniques: Recursive Feature Elimination (RFE) and Principal Component Analysis (PCA). By applying these methods, the research aims to optimize the input space for the LSTM models, reducing redundancy and improving generalization.
Models were trained to perform single-step forecasts of daily closing prices, and their performance was evaluated through statistical error metrics with Mean Absolute Percentage Error (MAPE) and Root Mean Squared Error (RMSE),  and a simulated trading strategy to assess practical effectiveness.
The results provide insights into the comparative strengths of different feature engineering approaches and dimensionality reduction methods, highlighting the trade-offs between model complexity, accuracy, and real-world applicability. This combined evaluation underscores the importance of thoughtful data preprocessing and feature optimization in building robust financial forecasting models


------MODELS TRAINED----
16 were trained in total for this research,
6 models (3 for S&P500 and 3 for FTSE100) for investigating the performance of the LSTM model when trained with 20, 10 and 5 years of data ---> data lenght
6 models (3 for S&P500 and 3 for FTSE100)for investigating the performance of the LSTM model, when trained with a PCA optimized dataset with 95&, 97% and 99% of variance retained --> PCA
6 models (3 for S&P500 and 3 for FTSE100)for investigating the performance of the LSTM model, when trained with a RFE optimized dataset with 13, 10 and 7 of selected features --> RFE
