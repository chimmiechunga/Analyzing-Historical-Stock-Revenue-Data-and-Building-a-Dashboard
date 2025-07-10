# Analyzing-Historical-Stock-Revenue-Data-and-Building-a-Dashboard
Extracting Tesla Stock Data Using yfinance
import yfinance as yf
import pandas as pd

# Download Tesla stock data
tesla_data = yf.download('TSLA', start='2010-01-01', end='2025-01-01')

# Reset the index
tesla_data.reset_index(inplace=True)

# Display first 5 rows
tesla_data.head(5)
