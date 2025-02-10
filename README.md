# Short-Term Stock Market Prediction Using Technical Indicators and Machine Learning

## Author
**Rashi Niyas P**  
**Email:** zda24m005@iitmz.ac.in  
**GitHub Repository:** [Stock Market Prediction](https://github.com/rashiniyasp/Stock-Market-Prediction-Using-Technical-indicators)

## Abstract
This project presents a machine learning approach for short-term stock market prediction using various technical indicators. Stock data was collected from Yahoo Finance and processed through feature engineering, including volume, volatility, trend, momentum, and price-based features. The data was normalized, and Principal Component Analysis (PCA) was applied for dimensionality reduction. Classification models like Logistic Regression, Random Forest, and XGBoost were trained and optimized using RandomizedSearchCV. The final evaluation was performed on unseen data from **May 29, 2024, to November 29, 2024**. Results show that engineered features significantly enhance predictive performance.

## 1. Introduction
Stock market prediction is crucial for investors aiming to make informed decisions. Traditional methods struggle with volatility, leading to the adoption of machine learning techniques. This project explores supervised learning algorithms to classify stock price direction, leveraging historical data and technical indicators to enhance predictive accuracy.

## 2. Problem Formulation
The project aims to predict stock price movement over a **30-day period** using binary classification:
- **Increase (1):** Price rises after 30 days.
- **Decrease (0):** Price falls after 30 days.

## 3. Description of Data
The dataset was collected using the **Yahoo Finance API**, covering **January 1, 2020, to November 30, 2024**. It includes:
- **Original Features:** Date, Adjusted Close, Close, High, Low, Open, Volume, Company.
- **Engineered Features:** Moving Averages, RSI, Volatility measures, Momentum indicators, Trend indicators, and Lagged Features.

### Data Processing Steps:
1. **Data Collection:** Retrieved stock prices, trading volumes, and financial metrics.
2. **Data Cleaning:** Handled missing values and outliers.
3. **Feature Engineering:** Computed technical indicators such as **Moving Averages, RSI, Bollinger Bands, and ATR**.

## 4. Methods and Analysis Approach
### 4.1 Feature Engineering
- **Volume Indicators:** Money Flow Index (MFI), On-Balance Volume (OBV).
- **Volatility Indicators:** Bollinger Bands (BB), Average True Range (ATR).
- **Momentum Indicators:** Relative Strength Index (RSI), Stochastic Oscillator.
- **Trend Indicators:** Simple Moving Average (SMA), Exponential Moving Average (EMA), MACD.

### 4.2 Data Preprocessing
- **Handling Missing Values:** K-Nearest Neighbors Imputer (k=2).
- **Normalization:** ATR/CLOSE × 100.
- **Feature Selection:** PCA retaining **95% variance**.

### 4.3 Model Selection
- **Logistic Regression:** Strong baseline for classification.
- **Random Forest:** Ensemble learning method for robustness.
- **XGBoost:** Gradient boosting for non-linear relationships.

### 4.4 Hyperparameter Tuning
**RandomizedSearchCV** was used for tuning parameters:
- **Logistic Regression:** C=0.249, penalty=l2.
- **Random Forest:** n_estimators=300, max_depth=None.
- **XGBoost:** learning_rate=0.107, max_depth=3.

## 5. Results and Discussion
### 5.1 Model Performance Evaluation
Performance metrics on the test dataset:
| Model | Accuracy | Precision | Recall | F1-Score | ROC AUC |
|--------|----------|-----------|--------|---------|---------|
| Logistic Regression | 50.75% | 57.28% | 42.47% | 48.78% | 51.18% |
| Random Forest | 55.21% | 55.26% | **99.12%** | 70.96% | 52.85% |
| XGBoost | **55.45%** | 55.36% | 99.76% | **71.20%** | **57.40%** |

- **XGBoost achieved the highest F1-score (71.20%) and ROC AUC (57.40%).**
- **Random Forest had high recall (99.12%) but low specificity.**
- **Logistic Regression performed the worst due to its linear nature.**

## 6. Conclusions
This study demonstrates the effectiveness of machine learning for short-term stock prediction. **XGBoost outperformed Logistic Regression and Random Forest**, indicating that tree-based models better capture market dynamics. Future improvements may include:
- **Deep Learning models (LSTMs, Transformers).**
- **Sentiment Analysis integration.**
- **More robust feature selection techniques.**

## References
1. Y. Alsubaie et al., "Cost-Sensitive Prediction of Stock Price Direction," *IEEE Access*, 2019.  
2. D. Mo and Y. Chen, "Financial Technical Indicators for Portfolio Building," *IEEE Access*, 2021.  
3. A. T. Haryono et al., "Stock Price Prediction Using Transformers and Technical Indicators," *IEEE Access*, 2023.  

---
### 📌 **How to Run the Code**
```bash
# Clone the repository
git clone https://github.com/rashiniyasp/Stock-Market-Prediction-Using-Technical-indicators
cd Stock-Market-Prediction-Using-Technical-indicators

# Install dependencies
pip install -r requirements.txt

# Run the script
python main.py
```
---
### 🔗 **Connect with Me**
- **GitHub:** [@rashiniyasp](https://github.com/rashiniyasp)
- **Email:** zda24m005@iitmz.ac.in
