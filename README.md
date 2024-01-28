# Automated Stock Data Dashboard

## Overview
This project involves creating an automated data dashboard that reads data about stock prices from the AlphaVantage API and produces corresponding charts and reports. The dashboard is produced by a reusable function called `generate_stocks_report()`.

## Requirements

### Function and Parameter Requirements
- The function should accept a stock symbol as a parameter input, with "NFLX" as the default symbol if not provided.
- The function should produce a data visualization of the stock prices over time and a summary report of key metrics.

### Validation Requirements
- The function should gracefully handle any errors if an invalid stock symbol is passed in and display a friendly error message.
- It should avoid unnecessary extra requests and handle API responses appropriately.

### Part I (Data Extraction)
- Real-time stock market data is fetched from the AlphaVantage API's "Daily Adjusted" endpoint in CSV format.
- Security measures are taken to handle the API key securely.

### Part II (Data Visualization)
- The function displays a chart of the closing prices over time with appropriate title and axis labels.
- Additionally, it can display a candlestick chart and a 50-day moving average trend line.

### Part III (Data Analysis)
- The function generates a report with details about the stock, including column names, number of rows, latest and earliest available dates, closing prices, 100-day high and low prices, and percentage change between the earliest and latest closing prices.

## Further Exploration
- Additional features can be implemented such as different chart types, additional data analysis metrics, and more.

## Usage
1. Clone this repository to your local machine.
2. Open the notebook in your preferred environment.
3. Update the AlphaVantage API key in the notebook.
4. Run the `generate_stocks_report()` function with your desired stock symbol to generate the dashboard.
