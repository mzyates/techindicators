
## List of functions

### sma

The sma function is the [simple moving average](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:moving_averages).  Two parameters are required: a Numpy array of prices, and the number of time periods for averaging.  The function returns the simple moving average as a numpy array.  Note that the length of the moving average will be shorter than the price series by N-1, where N is the period for averaging.

### ema

The ema function is the [exponential moving average](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:moving_averages).  Two parameters are required: a Numpy array of prices, and the number of time periods for averaging.  The function returns the simple moving average as a numpy array.  Note that the length of the moving average will be shorter than the price series by N-1, where N is the period for averaging.

### wma

The wma function calculates the [weighted moving average](https://www.fidelity.com/learning-center/trading-investing/technical-analysis/technical-indicator-guide/wma).  wo parameters are required: a Numpy array of prices, and the number of time periods for averaging.  The function returns the weighted moving average as a numpy array.  Note that the length of the moving average will be shorter than the price series by N-1, where N is the period for averaging.

### kama

The kama function is the [Kaufman adaptive moving average](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:kaufman_s_adaptive_moving_average).  Four parameters are required: a Numpy array of prices, the number of periods for the efficiency ratio calculation, the number of periods for the fastest exponential moving average constant, and the number of periods for the slowest exponential moving average constant.  The time periods are adjustable, but Kaufman originally suggested time periods of 10, 2, and 30 for the efficiency ration, fastest EMA, and slowest EMA, respectively.  The kama function returns the average as a Numpy array whose length is shorter than the price array by N-1, where N is the number of periods used for the efficiency ratio.

### atr

The atr function is [average true range (ATR)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:average_true_range_atr).  The function requires four parameters: an array of high prices, an array of low prices, and array of closing prices, and a time period for averaging.  The time period is adjustable, but 14 is typically used.  The average true range is returned as an array shorter than the price array by N-1, where N is the time period used for averaging.

### rsi

The rsi function calculates the [Relative Strength Index (RSI)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:relative_strength_index_rsi).  The function requires two parameters: an array of prices, and a number of time periods for averaging.  The number of time periods is adjustable, but 14 is typically used.  The RSI is returned as an array that is shorter than the price array by N, where N is the number of periods used for averaging.

### cci

The cci function calculates the [Commodity Channel Index (CCI)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:commodity_channel_index_cci).  The function requires four parameters: an array of high prices, and array of low prices, and array of closing prices, and a number of time periods for averaging.  The number of time periods is adjustable, but a value of 20 is typically used.  The function returns the calculated cci values in an array that is shorter than the length of the price array by N-1, where N is the number of periods used for averaging.

### adl

The adl function calculates the [Accumulation/Distribution Line (ADL)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:accumulation_distribution_line).  The function requires four parameters: an array of high prices, and array of low prices, and array of closing prices, and a trading volume.  The function returns the adl values as an array whose length is equal to the length of the price arrays.

### macd

The macd function calculates the [Moving Average Convergence/Divergence (MACD)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:moving_average_convergence_divergence_macd).  The function requires four parameters: an array of prices, a number of periods for the fast EMA, a number of periods for the slow EMA, and a number of periods for the signal line.  The function returns two arrays: the MACD Line and Signal Line.  The difference between the MACD Line and Signal Line can be used to calculate the MACD histogram.

### ppo

The ppo function calculates the [Percentage Price Oscillator (PPO)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:price_oscillators_ppo).  The function requires four parameters: an array of prices, a number of periods for the fast EMA, a number of periods for the slow EMA, and a number of periods for the signal line.  The function returns two arrays: the PPO Line and Signal Line.  The difference between the PPO Line and Signal Line can be used to calculate the PPO histogram.

### kelt

The kelt function calculates [Keltner Channels](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:keltner_channels).  The function requires six parameters, arrays of high prices, low prices, and closing prices, the number of periods for calculating the center line EMA, the multiple for the ATR, and the number of periods for calculating the ATR.  The function returns the lower, center, and upper lines of the Keltner Channels.

### rstd

The rstd function calculates a rolling [standard deviation](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:standard_deviation_volatility).  The function requires two parameters: an array of prices, and a number of periods used for calculating the standard deviation.  The function returns an array of the rolling standard deviation.

### boll

The boll function calculates the [Bollinger Bands<html>&reg;</html>](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:bollinger_bands).  The function requires four parameters: an array of prices, number of periods for calculating the center line SMA, multiplier for the standard deviation, and the number of periods used for calculating the rolling standard deviation.  The function returns the lower, center, and upper lines of the Bollinger Bands<html>&reg;</html>.

### trix

The trix function calculates the [TRIX indicator](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:trix).  The function requires three parameters: an array of prices, and a number of periods used for calculating the trimple EMA line, and the number of periods used for calculating the EMA of the signal.  The function returns the TRIX line and signal.

### stoch

The stoch function calculates the [Stochastic Oscillator](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:stochastic_oscillator_fast_slow_and_full).  The function requires six parameters: an array of high prices, an array of low prices, an array of closing prices, a look back period, a number of periods for calculating the %K moving average, and the number of periods for calculating the %D moving average.  The standard slow stochastic oscillator is calculated using the parameters (high,low,close,14,3,3).  The standard fast stochastic oscillator is calculated with the parameters (high,low,close,14,1,3).  Other look back and moving average periods may be selected to create a custom stochastic oscillator.

### vortex

The vortex function calculates the [Vortex Indicator](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:vortex_indicator).  The function requires four parameters: an array of high prices, and array of low prices, an array of closing prices, and a number of periods used for calculation.  The function returns the +VM and -VM indicators. 

### adx

The adx function calculates the [Average Directional Index (ADX)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:average_directional_index_adx). The function requires four parameters: an array of high prices, and array of low prices, an array of closing prices, and a number of periods used for calculation.  The function returns the positive directional indicator (+DI), negative directional indicator (-DI), and the ADX line. 

### aroon

The aroon function calculates the [Aroon Up/Down Indicators](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:aroon) and the [Aroon Oscillator](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:aroon_oscillator).  The function requires three parameters: an array of high prices, and array of low prices, and a number of periods for calculation.  The function returns the up indicator, down indicator, and oscillator.

### chand

The chand function calculated the [Chandelier Exit](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:chandelier_exit), which is a trailing stop loss based on a multiple of the ATR.  The function requires five parameters: high prices, low prices, closing prices, number of periods for ATR, the ATR multiple, and a string of either 'long' or 'short' to indicate which type of position is being held.

### roc

The roc function calculates the [Rate of Change (ROC)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:rate_of_change_roc_and_momentum).  The function requires two parameters: an array of prices and a number of periods for calculation.

### copp

The copp function calculates the [Coppock Curve](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:coppock_curve).  The Coppock curve is the weighted moving average (WMA) of the sum of two rates of change (ROC) calculated over two different time periods.  The function requires four parameters: an array of prices, a number of periods for the long ROC (14 is standard), a number of periods for the short ROC (11 is standard), and a number of periods for the WMA (10 is standard).

### force

The force function calculates the [Force Index](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:force_index).  The Force Index is an exponential moving average of the product of trading volume and the difference between closing price and the closing price of the previous period.  The force function requires three parameters: closing prices, trading volumes, and a number of periods.

### cmf

The cmf function calculates the [Chaikin Money Flow](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:chaikin_money_flow_cmf).  The function requires five parameters: high prices, low prices, closing prices, and a number of periods.  The default number of periods is 20, but this can be adjusted.  The cmf function returns the Chaikin Money Flow as an array.

### chosc

The chosc function calculates the [Chaikin Oscillator](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:chaikin_oscillator) given the parameters of: high prices, low prices, closing prices, volume, number of periods for shorter exponential moving average, and number of periods for longer exponential moving average.  The standard oscillator calculation uses 3 periods for the shorter EMA, and 10 periods for the longer EMA.

### emv

The emv function calculates the [Ease of Movement (EMV)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:ease_of_movement_emv) oscillator.  The function returns the ease of movement provided the parameters of high prices, low prices, volume, and a number of periods for calculation.  The standard number of periods is 14.

### mindx

The mindx function calculates the [Mass Index](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:mass_index).  The Mass Index is a measure of volatility based on a ratio of moving averages of the difference between high and low prices for each period.  When the Mass Index is high, there is an increased chance of a trend reversal.  The function requires three parameters: high prices, low prices, and a number of periods.  The standard number of periods is 25 and the standard trigger level for trend reversal is 27.

### mfi

The mfi function calculates the [Money Flow Index (MFI)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:money_flow_index_mfi). The MFI (also called volume weighted RSI), is an oscillator that uses the typical price and volume of each period. The mfi function requires parameters of high prices, low prices, closing prices, volume, and a number of periods for calculation. The standard number of periods is 14.

### nvi

The nvi function calculates the [Negative Volume Index (NVI](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:negative_volume_inde).  The single period percent change in price is added to the NVI on days when volume has declined from the previous day.  On days in which the volume has increased from the previous day, the NVI is left unchanged.  The signal line is an exponential moving average of the NVI.  The nvi function requires three parameters: closing prices, volume, and number of periods for EMA calculation.  The NVI and signal line are returned.

### obv

The obv function calculates the [On Balance Volume (OBV)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:on_balance_volume_obv).  The OBV is a running total of volume in which trading volume is added to the previous period's trading volume when price change is positive, and subtracted from the previous period's trading volume when price change is negative.  The obv function calculates the On Balance Volume given an array of closing prices and an array of trading volume.

### pvo

The pvo function calculates the [Percentage Volume Oscillator (PVO)](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:percentage_volume_oscillator_pvo).  The function requires four parameters: an array of volume, a number of periods for the fast EMA, a number of periods for the slow EMA, and a number of periods for the signal line.  The function returns two arrays: the PVO Line and Signal Line.  The difference between the PVO Line and Signal Line can be used to calculate the PVO histogram.

### kst

The kst function calculates the [Pring's Know Sure Thing (KST](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:know_sure_thing_kst) indicator line and signal line.  The KST indicator is based on the combined average rates of change in price on four different numbers of periods:

KST=SMA1(ROC1)+2∗SMA1(ROC2)+3∗SMA3(ROC3)+4∗SMA4(ROC4)

where "SMA" refers to the simple moving average, and "ROC" is the rate of change in price. The signal line is a simple moving average of KST. Since the number of periods for each of the 4 rates of change are adjustable, and the number of periods for each simple moving average is adjustable, the calculation of KST involves a lot of parameters. The standard values are 10, 15, 20, and 30 periods for calculation of ROC1, ROC2, ROC3, and ROC4, respectively. Standard vales are 10, 10, 10, 15, and 9 periods for SMA1, SMA2, SMA3, SMA4, and the signal line SMA, respectively. Therefore, the standard call to the kst function would be:

kst(price,10,15,20,30,10,10,10,15,9)

where "price" refers to an array of prices (typically closing prices are used).  The Jupyter notebook provides an example of the standard KST calculation and a plot of the results.
