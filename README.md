# Tesla Stock Forecasting Project
**Please either view the Jupyter notebook in Jupyter Lab or download the Tesla_LSTM.html file to explore the project. This is due to the implementation of interactive plots. Alternatively, you can view the project on my Kaggle page: [Tesla Stock Forecasting | Multi-Step Stacked LSTM](https://www.kaggle.com/code/guslovesmath/tesla-stock-forecasting-multi-step-stacked-lstm)**.

## Overview
This repository contains notebooks and data for a project on forecasting Tesla (TSLA) stock prices using multi-step stacked LSTM neural networks. The project includes a single-step ahead production model using a single LSTM and a multi-stacked LSTM model that predicts multiple days (a month in business days) into the future. The accompanying documentation provides an intuitive and mathematical background on LSTM networks, as well as insights into the use of stacked LSTMs and multistep forecasting for time series analysis.

## Data
- Historical stock price data for Tesla (TSLA).
- Data includes daily closing prices, open, high, low, volume, dividends, and stock splits.

## Models
1. **LSTM Single Step Ahead Model**
   - Implements a single LSTM model for one-step ahead stock price forecasting.
   - Forecasting two weeks into the future (in business days).
   - Data preprocessing, model training, and evaluation.

2. **Multi-Step Stacked LSTM Model**
   - Builds a multi-stacked LSTM model for forecasting multiple days into the future.
   - Maps n points to m points in the future (a month in business days).
   - In-depth analysis of model architecture, training process, and evaluation.

## Files
- **LSTM_Tesla_model.h5:** Trained weights for the single-step ahead LSTM model.
- **Multi_LSTM_Tesla_model.h5:** Trained weights for the multi-step stacked LSTM model.
- **Tesla_LSTM.ipynb:** Jupyter notebook for the project, covering data exploration, model building and implementation, and analysis.
- **Tesla_LSTM.html:** HTML file of the Jupyter notebook for project viewing with interactive plots.

## Dependencies
- Python: 3.11.5
- Libraries:
  - yfinance 0.2.32
  - pandas 2.1.1
  - numpy 1.26.2
  - scikit-learn 1.3.1
  - plotly 5.18.0
  - scipy 1.11.3
  - tensorflow 2.14.0
  - keras 2.14.0

## Data Sample

```plaintext
                 open      high       low     close      volume  dividends  stock splits
Date                                                                                     
2023-11-24  233.750  238.750  232.330  235.450   65125200        0.0          0.0
2023-11-27  236.890  238.330  232.100  236.080  112031800        0.0          0.0
2023-11-28  236.680  247.000  234.010  246.720  148549900        0.0          0.0
2023-11-29  249.210  252.750  242.760  244.140  135401300        0.0          0.0
2023-11-30  245.140  245.220  236.910  240.080  132353200        0.0          0.0
