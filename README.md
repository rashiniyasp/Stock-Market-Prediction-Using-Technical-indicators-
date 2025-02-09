# Stock-Market-Prediction-Using-Technical-indicators-
 Predicting short-term stock prices is a challenging yet vital task in financial markets.  This project leverages machine learning techniques to analyze historical stock  data and technical indicators to predict price movements in Indian and Tanzanian  markets.
 **ProblemFormulation**
 The models will be trained to make predictions over a 30- to 90-day period. The problem will be
 approached as classification task:
 • Classification Task: Determine the direction of price movements (up or down).
 **Description of Data**
 Historical stock data was collected using the Yahoo Finance API for the period from January 1, 2020,
 to November 30, 2024. Data preprocessing steps included:
 • Feature Columns:
 – Original: Adj Close, Close, High, Low, Open, Volume, Company.
 – Engineered: MA_5, Disparity_5, High_N, Low_N, %R, %K, %D, Momentum, Moving Average, Rolling Std, Upper Boundary, Lower Boundary and many more.
Target Variable:
**Defined as Target**, representing the direction of price movement (1 for increase, 0
 for decrease).
 **Companies Analyzed**
 Indian Companies: ADANIENT.NS, ASIANPAINT.NS, BAJFINANCE.NS, BHAR
TIARTL.NS, CIPLA.NS, COALINDIA.NS, DRREDDY.NS, EICHERMOT.NS,
 GRASIM.NS, HCLTECH.NS, HDFCBANK.NS, HINDUNILVR.NS, ICICIBANK.NS, IN
DUSINDBK.NS, INFY.NS, ITC.NS, KOTAKBANK.NS, LT.NS, M&M.NS, MARUTI.NS,
 NESTLEIND.NS, POWERGRID.NS, RELIANCE.NS, SBIN.NS, SUNPHARMA.NS,
 TATASTEEL.NS, TCS.NS, TECHM.NS, ULTRACEMCO.NS, WIPRO.NS.
 Tanzanian Companies: ACA, CRDB, DCB, MBP, MCB, NMB, PAL, TBL, TCC, TOL,
 TTP
