
## List of functions

### sma

The sma function is the [simple moving average](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:moving_averages).  Two parameters are required: a Numpy array of prices, and the number of time periods for averaging.  The function returns the simple moving average as a numpy array.  Note that the length of the moving average will be shorter than the price series by N-1, where N is the period for averaging.

### ema

The ema function is the [exponential moving average](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:moving_averages).  Two parameters are required: a Numpy array of prices, and the number of time periods for averaging.  The function returns the simple moving average as a numpy array.  Note that the length of the moving average will be shorter than the price series by N-1, where N is the period for averaging.

### kama

The kama function is the [Kaufman adaptive moving average](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:kaufman_s_adaptive_moving_average).  Four parameters are required: a Numpy array of prices, the number of periods for the efficiency ratio calculation, the number of periods for the fastest exponential moving average constant, and the number of periods for the slowest exponential moving average constant.  The time periods are adjustable, but Kaufman origibnally suggested time periods of 10, 2, and 30 for the efficiency ration, fastest EMA, and slowest EMA, respectively.  The kama function returns the average as a Numpy array whose length is shorter than the price array by N-1, where N is the number of periods used for the effciency ratio.

### atr

The atr function is [average true range](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:average_true_range_atr)  The function requires four parameters: an array of high prices, an array of low prices, and array of closing prices, and a time period for averaging.  The time period is adjustable, but 14 is typically used.  The average true range is returned as an array shorter than the price array by N-1, where N is the time period used for averaging.

### rsi

The rsi function calculates the [Relative Strength Index](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:relative_strength_index_rsi).  The function requires two parameters: an array of prices, and a number of time periods for averaging.  The number of time periods is adjustable, but 14 is typically used.  The RSI is returned as an array that is shorter than the price array by N, where N is the number of periods used for averaging.

### cci

The cci function calculates the [Commodity Channel Index](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:commodity_channel_index_cci).  The function requires four parameters: an array of high prices, and array of low prices, and array of closing prices, and a number of time periods for averaging.  The number of time periods is adjustable, but a value of 20 is typically used.  The function returns the calculated cci values in an array that is shorter than the length of the price array by N-1, where N is the number of periods used for averaging.

### adl

The adl function calculates the [Accumulation Distribution Line](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:accumulation_distribution_line).  The function requires four parameters: an array of high prices, and array of low prices, and array of closing prices, and a trading volume.  The function returns the adl values as an array whose length is equal to the length of the price arrays.
