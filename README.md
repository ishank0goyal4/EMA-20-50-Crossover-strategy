# EMA-20-50-Crossover-strategy

## Exponential moving average(EMA)
The EMA is created to improve on the idea of a simple moving average. It gives more weight to the most recent price data. The shorter time span average is more sensitive to the price change of underlying, and the longer time span average is less sensitive. Hence we will use their crossover there to create buy and sell signals. 


## Trade Setup
When a short-term moving average(20 days) crosses above a longer-term moving average(50 days), this will confirm bullish momentum. Thus It will close our previous sell position if any, and a fresh buy signal will be created.
When a short-term moving average(20 days) crosses below a longer-term moving average(50 days), this will confirm a bearish momentum. Thus It will close our previous buy position if any, and a fresh sell signal will be created.


I have used the yfinance library to download open, high, low. Close, volume historical data of S&P 500 index, backtesting library to create a strategy   

Note: The graph and trades I have added  is based on june 2019 to june 2021 data.

