## 📈 Tesla Stock Price Prediction

This project focuses on predicting the stock prices of Tesla (and AMD) by integrating sentiment analysis of Reddit posts with market data from Yahoo! Finance, using Recurrent Neural Networks (RNN) with Long Short-Term Memory (LSTM) layers. Two distinct methods are employed to collect data for sentiment analysis:

- **Method 1**: Use of the Reddit API.
- **Method 2**: Use of .zst-compressed datasets.

### Project Overview

- Extracting/loading Reddit post titles depending on the method.
- Performing sentiment analysis on the data using the VADER model.
- Merging sentiment scores with historical market data from Yahoo! Finance.
- Building and training RNN + LSTM models to predict stock closing prices.
- Evaluating model performance using RMSE and MAPE.

### 🔍 Method Overview

#### 📌 Method 1: Use of the Reddit API.
- See `API method explanation.pdf` for details.

**Tesla:**
- Train RMSE: **9.56**
- Test RMSE: **12.00**
- Test MAPE: **0.18**

#### 📌 Method 2: Use of .zst-compressed datasets.
- Uses `zstandard` library to decompress Reddit `.zst` files for both TSLA and AMD_Stock subreddits.

**Tesla:**
- Train RMSE: **9.84**
- Test RMSE: **7.54**
- Test MAPE: **0.15**

**AMD:**
- Train RMSE: **2.40**
- Test RMSE: **3.44**
- Test MAPE: **0.17**

### Summary
Overall, Method 2 shows improved generalization for Tesla stocks.

### 📁 Data Sources

- Reddit posts: from r/TSLA and r/AMD_Stock
- Market data: from Yahoo Finance's API via the `yfinance` Python package
