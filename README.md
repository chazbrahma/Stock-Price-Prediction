# Stock Price Prediction Using Machine Learning

This project focuses on predicting future stock prices for NASDAQ (NDAQ) using machine learning regression techniques. It demonstrates an end-to-end machine learning pipeline applied to financial time series data. The approach includes data preprocessing, feature engineering, model training, and evaluation. The project is implemented in Python within a Jupyter Notebook environment.

# Project Overview

The aim of this project is to develop a predictive model that forecasts stock prices based on historical data. The dataset consists of historical stock prices for NASDAQ (NDAQ), which is processed and used to train a regression-based machine learning model. The model provides baseline predictions with performance evaluated on unseen data.

# Dataset Details

The dataset `NDAQ_data.csv` contains daily stock price data for NASDAQ. It includes columns such as Date, Open, High, Low, Close, and Volume. The data spans from 8th Feb 2013 to 7th Feb 2018. Preprocessing includes handling missing values and converting date columns to datetime format.

# Methodology

The project follows these steps:
- Data preprocessing: handling missing values, sorting chronologically
- Feature engineering: creating lag features and technical indicators such as SMA, EMA, Rolling Std Dev, RSI, Bollinger Bands, OBV, and more
- Model training: using a Linear Regression model as a baseline
- Model evaluation: assessing performance with MSE, RMSE, and MAE

# Model Results and Evaluation

Training Set Metrics
- Mean Squared Error (MSE): 0.07076469854616008  
- Root Mean Squared Error (RMSE): 0.2660163501481818  

Testing Set Metrics
- Mean Squared Error (MSE): 0.07076469854616008  
- Root Mean Squared Error (RMSE): 0.2660163501481818  

These metrics indicate consistent performance between the training and testing datasets, with minimal overfitting.

A visual comparison between the actual and predicted prices can be seen below:

![actual_vs_predicted_scatter](https://github.com/user-attachments/assets/75ed0df5-e773-4a71-a60c-2050b6084c3b)

The scatter plot presents a comparison between the actual stock prices and the prices predicted by the model. The horizontal axis represents the actual prices, while the vertical axis shows the predicted values. The close alignment of the data points along the diagonal line indicates a strong correlation between the two sets of values, demonstrating that the model is performing well in predicting stock prices with a high degree of accuracy. The tight clustering of points around the line suggests minimal error and reliable predictive capability.

# Installation and Setup

1. Clone the repository (optional if you upload zipped files):  
   `git clone https://github.com/chazbrahma/Stock-Price-Prediction.git`

2. Install required dependencies:  
   `pip install -r requirements.txt`

3. Launch the Jupyter Notebook:  
   `cd notebooks`  
   `jupyter notebook StockMarketPredictionV1_0.ipynb`

# Usage Instructions

Follow the Jupyter Notebook to explore data preprocessing, feature engineering, model training, and evaluation. Modify and extend the notebook for additional datasets or more advanced models.

# Future Enhancements

Planned improvements include:
- Implementing LSTM, XGBoost, or ARIMA models
- Hyperparameter optimization (GridSearchCV or Optuna)
- Integration with live data APIs (yFinance or Alpaca)
- Deployment as an interactive web app using Streamlit

# Author

Chazin Brahma  
- [GitHub](https://github.com/chazbrahma)  
- [LinkedIn](https://www.linkedin.com/in/chazin-brahma-684197292/)
