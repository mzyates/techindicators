# techindicators
Python functions to calculate technical indicators from stock price data using Numpy.  A Jupyter notebook is also included demonstrating the calculation of technical indicators and plotting the resulting data.

## Purpose

The Python functions and the associated Jupyter notebook are used to calculate various technical indicators (such as various moving averages, relative strength index (RSI), movering average convergence/divergence (MACD), etc) from a time series of open, high, low, close (OHLC) prices of stocks or other securities. A full list of the available functions is given in the documentation. Price data in comma separated variable format is imported as Numpy arrays. The technical indicator functions rely on Numpy for calculations.

The code was written for those who would rather use Numpy matrices and arrays rather than Pandas dataframes for technical analysis calculations.  The Pandas library is not required.

## Using the functions

The documentation file has a list of the included function names along with a brief description of their use.  Links are provided in the documentation file for obtaining more information.  An example Jupyter notebook has been created to demonstrate the use of the functions, plotting data, and printing results.  To use the example notebook, download the following three files: techindicators.py, example_data.csv, and example_notebook.ipynb.  Place all three files in the same directory.  Then, open the example notebook file using the Jupyter client in order to execute and modify the code in the notebook file.

NOTE: The techindicators.py code was written in Python version 3.6.  The functions in techindicators.py depend on Numpy.  The code in the Jupyter notebook also depends on Matplotlib, Datetime, and mpl_finance.

All the necessary modules may be installed using pip, with the exception of mpl_finance.  The mpl_finance module can be found at:

https://github.com/matplotlib/mpl_finance

and installed using:

`pip install https://github.com/matplotlib/mpl_finance/archive/master.zip`
