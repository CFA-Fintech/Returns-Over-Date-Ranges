# Returns Over Date Ranges
This program reads daily stock data from a CSV, trims extraneous columns, converts date strings to datetime objects, sets the datetimes as the index, and calculates and plots returns for specified date ranges.

Harold's manager wants him to analyze the last 10 years of historical price data for Advanced Micro Devices (AMD), and then plot the daily returns over the last 1-, 3-, 5-, and 10-year periods. His manager wants to see the differences in average daily returns for each time period to determine whether a short- or long-term perspective should be used in prospecting AMD as a potential investment opportunity.

Use the following instructions to help Harold analyze the last 10 years of AMD stock data.

## Instructions
Complete the following steps.

  1. Import the necessary libraries and dependencies.

  1. Read in `amd_stock_data.csv` as a Pandas DataFrame.

  1. Display summary statistics of the input data to get a feel for your data.

  1. Drop the `volume`, `open`, `high`, and `low` columns.

  1. Set the `date` column as the DataFrame index.

  1. Drop the extra `date` column. (The index can now replace it.)

  1. Calculate daily returns.

  1. Use `loc()` to select subsets from the DatetimeIndex to create date ranges of 1, 3, 5, and 10 years. Remember that you can select date ranges using label indexing: `loc[start_date:end_date]`.

  1. Output summary statistics for each 1-, 3-, 5-, and 10-year subset.

  1. Plot daily return charts for each 1-, 3-, 5-, and 10-year subset.

  1. Formulate insights regarding the variation in average daily returns for each time period.

## Hint

Analyze the average daily returns from a numerical standpoint. Which time period has the highest average daily return and which has the lowest? What are the implications of this?

What are the average daily returns over each date range?
1 Year = 0.004538 or 4.53%
3 Year = 0.003455 or 3.45%
5 Year = 0.002304 or 2.30%
10 Year = 0.001488 or 1.49%

What insights could this provide in regards to wanting to trade AMD stock in the long-term vs. short-term?  

Based on the varying distributions of daily returns over 1 Year, 3 Year, 5 Year, and 10 Year periods, it would appear at though trading AMD in the short-term would more be profitable.
