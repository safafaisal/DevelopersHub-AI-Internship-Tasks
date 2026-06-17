# AAPL Next-Day Closing Price Prediction

## Objective

Predict Apple’s (AAPL) next-day closing price from its Open, High, Low, and Volume, using Linear Regression.

## Dataset

5 years of AAPL daily data, fetched via the `yfinance` library.

## Tools

Python, yfinance, pandas, scikit-learn, matplotlib

## Approach

- Created a `Next_Close` target by shifting `Close` one day back
- Split data chronologically (80% train / 20% test, no shuffling)
- Trained a Linear Regression model
- Evaluated with MAE, RMSE, R²

## Results

- MAE: 3.37
- RMSE: 4.50
- R² (test): 0.973

## Insight

Today’s price is a strong predictor of tomorrow’s price, which is why accuracy is high — but the model can’t anticipate sudden news-driven jumps.

## How to Run

Open `stock_price_prediction.ipynb` in Jupyter and run all cells in order.