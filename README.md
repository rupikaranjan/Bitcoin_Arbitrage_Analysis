# Bitcoin_Arbitrage_Analysis
This Application collects , prepare and analyze Bitcoin coin data across two exchanges (Bitstamp and Coinbase) and tells if there are any arnitrage opportunities fot it.

---

## Technologies

This application works on python 3.7 and uses following libraries:

* [fire](https://github.com/google/python-fire) - For the command line interface and entry-point.

* [questionary](https://github.com/tmbo/questionary) - For user interactive inputs and dialogs.

* [matplotlib](https://github.com/matplotlib/matplotlib.git) - For creating static, animated, and interactive visualizations.

---

## Installation Guide

Follow the following instructions before using the application.

```python
  pip install fire
  pip install questionary
  pip install -U matplotlib
```
---

## Detailed Explanation

Bitcoin Arbitrage Analysis has following three phases

1. Data Collection
2. Data Preparation
3. Data Analysis

### Data Collection
Dataframes `bitstamp` and `coinbase` is created using the Pandas `read_csv` function and the `Path` module by importing the data from `bitstamp.csv` file and `coinbase.csv` file. The `Timestamp` column is set as index column

### Data Preparation
Collected data is then prepared and cleaned for analysis by following the steps below for both `bitstamp` and `coinbase` dataframes:

1. Replaced all `NaN`, or missing, values in the DataFrame with mean of that column.

2. Using the `str.replace` function to remove the dollar signs ($) from the values in the Close column.

3. Convert the data type of the Close column to a `float`.

4. Review the data for duplicated values, and dropping them.






