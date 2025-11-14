# Time-Series-
Investment Trend Forecasting using ARIMA, Prophet & Hybrid Models

Project Overview
This project focuses on predicting investment trends and generating intelligent trade decisions using advanced time-series forecasting models including ARIMA, SARIMA, Prophet, and LSTM.
The goal is to build a framework that helps investors make data-driven buy/sell decisions with maximum returns and minimal losses.
The project integrates both statistical forecasting and technical indicators (like Bollinger Bands, trailing stops, and minimum margin thresholds) to simulate practical market decision-making.

Dataset
Source: Investment/market data stored in invest.xlsx
Features: Date, Open, High, Low, Close, Volume
Frequency: Daily records
Preprocessing: Missing values handled, volume and percentage columns cleaned, and data normalized for model input.

Methodology
ARIMA model: Used for univariate forecasting based on historical closing prices. Captures short-term autocorrelations. 
Evaluated using RMSE and MAPE
