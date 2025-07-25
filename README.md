# 📊 Stock Screening

A Python script to monitor stock performance by comparing the **current market price** against predefined **base** and **support** levels.

## 🔍 Features

- Real-time price retrieval using `yfinance`
- Percentage change calculation from base and support prices
- Color-coded output for quick visual analysis
- Customizable stock list and thresholds

## 🛠 Requirements

- Python 3.x
- `pandas`
- `yfinance`
- `jinja2` (required for styled output in Jupyter Notebooks)

## 🚀 Usage Example

```python
from stock_screening import analyze_stocks           # analyze last close price
from stock_screening import analyze_stocks_realtime  # analyze realtime stock price

stocks = ["BBCA.JK", "BBRI.JK", "BMRI.JK", "BBNI.JK"]
base_prices = [7400, 3360, 4350, 3670]
support_prices = [8300, 3650, 4650, 3950]

# Analyze last close price
analyze_stocks(stocks, base_prices, support_prices)

# Analyze realtime stock price
analyze_stocks_realtime(stocks, base_prices, support_prices)