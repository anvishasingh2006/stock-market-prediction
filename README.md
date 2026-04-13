# stock-market-prediction
ML pipeline to predict AAPL stock direction using RSI, MACD, and Bollinger Bands. Backtested across Logistic Regression, Random Forest, and HistGradientBoosting.

# Stock Direction Prediction & Backtesting (AAPL)

Predicts next-day stock movement (up/down) using technical indicators and
compares three ML classifiers with a simple backtesting strategy.

## Dataset
~2,500 trading days of AAPL historical data (2016–2025)

## Features engineered
RSI (14-day), MACD, Bollinger Bands, MA10, MA50, Volatility, Volume Change, Trend

## Models
| Model | CV Accuracy | ROC-AUC |
|---|---|---|
| Logistic Regression | — | — |
| Random Forest | — | — |
| Hist Gradient Boosting | — | — |

## Backtesting (threshold = 0.52)
| Model | Trades | Win Rate | Final Return |
|---|---|---|---|
| Logistic Regression | 89 | 0.629 | 0.979x |
| Random Forest | 21 | 0.524 | 1.029x |
| Hist Gradient Boosting | 92 | 0.598 | 0.945x |

## How to run
````bash
pip install pandas numpy scikit-learn matplotlib seaborn
````
Then open `stock_prediction.ipynb` in Jupyter Notebook.
