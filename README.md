# Investment Trend Forecasting using ARIMA, Prophet & Hybrid Models

## Project Overview  
This project focuses on **predicting investment trends** and **generating intelligent trade decisions** using advanced time-series forecasting models — including **ARIMA**, **SARIMA**, **Prophet**, and **LSTM**.  
The goal is to build a framework that helps investors make data-driven buy/sell decisions with **maximum returns and minimal losses**.  

The project integrates both **statistical forecasting** and **technical indicators** (like **Bollinger Bands**, **trailing stops**, and **minimum margin thresholds**) to simulate practical market decision-making.

---

## Dataset  
- **Source:** Investment/market data stored in `invest.xlsx`  
- **Features:** Date, Open, High, Low, Close, Volume  
- **Frequency:** Daily records  
- **Preprocessing:** Missing values handled, volume and percentage columns cleaned, and data normalized for model input.

---

## 🧠 Methodology  

### 1. **ARIMA / SARIMA Models**
Used for univariate forecasting based on historical closing prices.  
- Captures short-term autocorrelations  
- Evaluated using RMSE and MAPE  

### 2. **Prophet Model**
Applied to capture **trend + seasonality + holidays**, offering explainable and fast forecasting.  
- Suitable for daily investment data  
- Provides flexible changepoint detection  

### 3. **LSTM Model**
For sequential deep learning forecasting, especially useful for capturing long-term dependencies.  
- Built with TensorFlow/Keras  
- Optimized with RMSE and validation loss  

### 4. **Decision Layer (Trading Logic)**
Integrated investment logic with:
- **Bollinger Bands** for volatility-based signal generation  
- **Minimum Margin Thresholds** to ensure profit on upward/downward trends  
- **Trailing Stop Mechanism** to dynamically adjust stop-loss levels  

---

## Model Comparison
| Model | Strength | Weakness | Usage |
|--------|-----------|-----------|--------|
| **ARIMA** | Good for linear stationary data | Poor with trend shifts | Baseline |
| **Prophet** | Handles seasonality and changepoints | May overfit small datasets | Intermediate |
| **LSTM** | Captures non-linear patterns | Requires more data and tuning | Advanced |

---

 Futuristic Approach  
The project sets the foundation for a **hybrid AI-based investment system**.  
Future plans include:
- Combining **Prophet + LSTM (Hybrid model)** for enhanced accuracy  
- **Backtesting strategies** with historical performance  
- Integrating with **real-time APIs (Yahoo Finance, Alpha Vantage)**  
- Deploying interactive dashboards (Streamlit / Flask) for visualization  
- Building automated **trade signal generators**  

---

## ⚙️ Installation & Usage
```bash
# Clone the repository
git clone https://github.com/<your-username>/Investment-Forecasting.git
cd Investment-Forecasting

# Install dependencies
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook Invest.ipynb
```

---

## Results & Visualization
- Time-series decomposition of trends and seasonality  
- Forecast plots for ARIMA, Prophet, and LSTM  
- Comparison of predicted vs. actual closing prices  
- Signal-based performance curves for buy/sell strategy  

---

## Conclusion  
The notebook demonstrates how combining **statistical forecasting** and **machine learning** can provide actionable insights for investments.  
By integrating forecasting with technical trading logic, this project moves a step closer to **automated portfolio intelligence**.  


