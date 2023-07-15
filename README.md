# :chart_with_upwards_trend: Mean-Reversion-Strategy
This project is an example of implementing a mean reversion strategy using Python. The project works on a portfolio that includes the tickers 'CPER', 'TLT', 'TTT', 'UUP', and 'VXX'.

## Project Objective
The objective of this project is to understand the correlation between the given stocks and apply a mean reversion strategy based on this correlation. The project evaluates the effectiveness of the strategy using statistical methods such as cointegration test, ADF test, and z-score calculation.

## Requirements
The project requires the following software and packages to be installed:

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- yfinance
Make sure these packages are installed. If they are not installed, you can install them using the following commands:  
``` pip install pandas numpy matplotlib seaborn statsmodels yfinance ```


## Project Steps
1. Data Collection: Collect the stock data to be used for the project. In this example, we will be using the yfinance library to fetch the daily closing prices. You can start by fetching the data for the respective tickers.

2. Data Analysis: Load the stock data and use a heatmap to analyze the correlation. Select the pair with the highest correlation and proceed with the mean reversion strategy based on that pair.

3. Cointegration Test: Apply the cointegration test to determine if the selected pair is cointegrated. This test helps determine if two series are in a long-term equilibrium relationship.

4. ADF Test: Apply the ADF test to the series that passed the cointegration test. This test checks for the stationarity property of the time series. Stationarity is the foundation of the mean reversion strategy.

5. Z-Score Calculation: Calculate the z-score using the mean and standard deviation of the two series. This is a measure of how far apart the two series are.

6. Ratio Calculation: Calculate the ratio between the two series and compute an average ratio using the rolling window method. This will be used to determine entry and exit points.

7. Trading Strategy: Monitor how far the obtained ratio deviates from the average ratio. If the ratio deviates beyond a certain threshold, a mean reversion strategy can be applied.

8. Visualization of Results: Visualize the trading transactions and the resulting profit/loss to evaluate the performance of the strategy.

## File Structure
* main.ipynb: This is the main application file of the project. This file follows the mentioned steps to implement the strategy and display the results.
* README.md: This file contains the description of the project and instructions for usage.

### Note
This project is presented as an example of implementing a strategy in financial markets. Be cautious and perform your own research when making actual trading or investment decisions.
