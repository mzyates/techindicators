# techindicators
The techindicators repository provides tools for technical analysis of open/high/low/close (OHLC) stock price data.  The techindicators.py code contains Python 3.6 functions to calculate a variety of technical indicators (moving averages, RSI, MACD, CCI, etc.) using the Numpy library.  The associated Jupyter notebook demonstrates the use of all of the functions included in techindicators.py.  Plots shown in the Jupyter notebook were created using Matplotlib and the mpl_finance module.

## Why create another technical analysis tool?

There are a number of tools already available for technical analysis using Python.  Most of them involve the use of the [Pandas](http://pandas.pydata.org/) data analysis library and/or the Python wrapper for the technical analysis library [TA-lib](http://www.ta-lib.org/).  So why re-invent the wheel?  The goal of writing this code is to simplify technical analysis of stock price data using the standard tools for numerical calculation with Python.  If you already know something about numerical calculations in Python with Numpy, using Pandas will seem foreign.  If you already know something about Python coding, the use of Ta-lib will likely make it more difficult to write your own code to do custom technical analysis.

The techindicators repository is Python-centric.  Numpy is the only dependency of the Python functions contained in techindicators.py.  The Jupyter notebook uses Matplotlib for plotting (the mpl_finance module is required for OHLC candlestick charts since Matplotlib decided to deprecate the finance module).

## Using the functions

If you are unfamiliar with Python, the easiest way to get started is to install the latest version of the [Anaconda distribution](https://docs.anaconda.com/anaconda/install/) for Python 3.6.  Anaconda is available for Windows, MacOS, and Linux operating systems and will provide everything need to run the technindicators code with the exception of mpl_finance.  The mpl_finance module can be found at:

https://github.com/matplotlib/mpl_finance

and installed using:

`pip install https://github.com/matplotlib/mpl_finance/archive/master.zip`

The documentation file has a list of the included function names along with a brief description of their use.  Links are provided in the documentation file for obtaining more information.  An example Jupyter notebook has been created to demonstrate the use of the functions, plotting data, and printing results.  To use the example Jupyter notebook, download the following three files: techindicators.py, example_data.csv, and example_notebook.ipynb.  Place all three files in the same directory.  Then, open the example notebook file using the Jupyter client in order to execute and modify the code in the notebook file.

NOTE: The techindicators.py code was written in Python version 3.6.
