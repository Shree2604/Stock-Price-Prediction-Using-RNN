# 📈 Stock Price Prediction Using RNN 📉

## Overview:
Discover the future of stock market gains! Predict Tata Motors' closing prices with LSTM, leveraging past data from Yahoo Finance.

## Libraries/Frameworks:
- **pandas_datareader:** Extract stock price datasets.
- **numpy:** Handle arrays efficiently.
- **pandas:** Manage data frames effortlessly.
- **MinMaxScaler:** Scale data for optimal performance.
- **Sequential:** Construct the ML model.
- **Dense:** Layer where each neuron receives input from all previous layer neurons.
- **LSTM:** Layer where each neuron receives input from all past layers.
- **Dropout:** Reduce overfitting by randomly selecting neurons.
- **matplotlib.pyplot:** Visualize data with graphs.

## Dataset link: https://finance.yahoo.com/quote/TTM/history?p=TTM
This dataset contains all the previous record of stock price of Tata Motors Company.
## To use the dataset in the code you can use this command

<code> code
import yfinance as yf
import datetime as dt
df = yf.download('TTM', dt.datetime(2012,1,1) , dt.datetime(2023,1,7)) 
</code>


## ML Model Details:
- **LSTM (Long short-term memory)**
  - **RMSE:** 0.9894
  - **Activation Functions:** Nadam
  - **Input Size:** (60, 1)
