# Stock Market Prediction Using Technical Indicators

Predicting short-term stock prices is a challenging yet vital task in financial markets. This project leverages machine learning techniques to analyze historical stock data and technical indicators to predict price movements in Indian and Tanzanian markets.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Problem Formulation](#problem-formulation)
3. [Data Description](#data-description)
4. [Feature Engineering](#feature-engineering)
5. [Companies Analyzed](#companies-analyzed)
6. [Usage](#usage)
7. [Contributing](#contributing)
8. [License](#license)

---

## Project Overview

This project aims to predict short-term stock price movements using machine learning models. By analyzing historical stock data and technical indicators, the models determine whether the price will increase or decrease over a 30- to 90-day period.

---

## Problem Formulation

The problem is approached as a **classification task**:
- **Objective**: Predict the direction of price movements (up or down).
- **Target Variable**: Defined as `Target`, where:
  - `1` indicates an increase in price.
  - `0` indicates a decrease in price.

---

## Data Description

Historical stock data was collected using the **Yahoo Finance API** for the period from **January 1, 2020, to November 30, 2024**. The dataset includes the following columns:

### Feature Columns:
- **Original Features**: Adj Close, Close, High, Low, Open, Volume, Company.
- **Engineered Features**: MA_5, Disparity_5, High_N, Low_N, %R, %K, %D, Momentum, Moving Average, Rolling Std, Upper Boundary, Lower Boundary, and many more.

### Target Variable:
- `Target`: Represents the direction of price movement (1 for increase, 0 for decrease).

---

## Feature Engineering

To enhance model performance, several technical indicators were engineered from the raw data. These include:
- Moving averages (e.g., MA_5).
- Disparity indices.
- Oscillators (e.g., %R, %K, %D).
- Momentum indicators.
- Bollinger Bands (Upper and Lower Boundaries).

---

## Companies Analyzed

### Indian Companies:
- ADANIENT.NS, ASIANPAINT.NS, BAJFINANCE.NS, BHARTIARTL.NS, CIPLA.NS, COALINDIA.NS, DRREDDY.NS, EICHERMOT.NS, GRASIM.NS, HCLTECH.NS, HDFCBANK.NS, HINDUNILVR.NS, ICICIBANK.NS, INDUSINDBK.NS, INFY.NS, ITC.NS, KOTAKBANK.NS, LT.NS, M&M.NS, MARUTI.NS, NESTLEIND.NS, POWERGRID.NS, RELIANCE.NS, SBIN.NS, SUNPHARMA.NS, TATASTEEL.NS, TCS.NS, TECHM.NS, ULTRACEMCO.NS, WIPRO.NS.

### Tanzanian Companies:
- ACA, CRDB, DCB, MBP, MCB, NMB, PAL, TBL, TCC, TOL, TTP.

---

## Usage

To use this project:
1. Clone the repository:
   ```bash
   git clone https://github.com/rashiniyasp/Stock-Market-Prediction-Using-Technical-indicators.git
