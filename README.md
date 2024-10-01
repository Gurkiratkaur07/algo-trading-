

### **Crypto Trading Bot using Binance API with Python**

This project is a crypto trading bot that interacts with the Binance API to fetch real-time data for the BTC/USDT pair, perform technical analysis using the Parabolic SAR (Stop and Reverse) indicator, and place automated buy/sell orders based on the analysis.

#### **Key Features:**

- **Data Collection**:
  - Utilizes the Binance API to retrieve historical and real-time candlestick data for the `BTCUSDT` pair with a specified interval (e.g., 1 day).
  - WebSocket connections are used to stream real-time data and update the dataset.

- **Technical Analysis**:
  - Employs the TA-Lib library to calculate the Parabolic SAR (Stop and Reverse) indicator for analyzing trends and generating buy/sell signals.

- **Automated Trading**:
  - Implements a `PlaceOrder` class to manage and execute buy/sell orders through the Binance API.
  - Includes methods for market order placements (`buy()` and `sell()`) based on real-time analysis.
  - Uses HMAC-SHA256 for creating secure signatures to authenticate API requests.

#### **Functionality**:

- **Data Processing**: 
  - Fetches data using `requests` and updates the DataFrame with real-time price data via WebSocket connections.
  
- **Trading Strategy**:
  - The bot continuously monitors the market and calculates the Parabolic SAR for trend analysis.
  - Automatically executes buy/sell orders when the conditions are met.

#### **Technologies Used**:
- **Python** for core programming
- **Binance API** for data retrieval and order placement
- **TA-Lib** for technical analysis
- **Pandas** for data manipulation
- **Websockets** for real-time data streaming

This project showcases how to integrate real-time cryptocurrency trading with Python, making it a comprehensive example of building an automated trading bot using APIs and technical analysis tools. 

