# Buy Sell Signal Low TF MT4

This is a custom indicator for MetaTrader 4 that provides buy and sell signals based on certain conditions. It uses the Simple Moving Average (SMA) and the Commodity Channel Index (CCI) to determine the signals.

## Indicator Parameters

- `smma13_period`: Period for the 13-period Simple Moving Average (SMA)
- `smma21_period`: Period for the 21-period Simple Moving Average (SMA)
- `smma35_period`: Period for the 35-period Simple Moving Average (SMA)
- `cci_period`: Period for the Commodity Channel Index (CCI)

## Indicator Buffers

- `BuyBuffer[]`: Buffer for storing buy signals
- `SellBuffer[]`: Buffer for storing sell signals
- `AlertBuffer[]`: Buffer for storing alert signals

## Indicator Initialization

The indicator initializes by mapping the indicator buffers and setting the indicator lines. The indicator lines are drawn as arrows on the chart. The name for the DataWindow and the indicator subwindow label is set as 'Buy Sell Signal Low TF MT4'.

## Indicator Calculation

The indicator calculates the buy and sell signals based on the given parameters and the current market data. It loops through the available data and checks the conditions for generating the signals.

If the CCI is greater than 0 and higher than the SMAs, a buy signal is generated. The buy signal is represented by a value calculated from the low price of the current bar. An alert signal is also generated, represented by a value calculated from the high price of the current bar.

If the CCI is less than 0 and lower than the SMAs, a sell signal is generated. The sell signal is represented by a value calculated from the high price of the current bar. An alert signal is also generated, represented by a value calculated from the low price of the current bar.

If none of the conditions are met, the buy, sell, and alert signals are set to EMPTY_VALUE, indicating no signal.

## Product Description

This code represents a custom indicator for MetaTrader 4 that provides buy and sell signals based on the Simple Moving Average (SMA) and Commodity Channel Index (CCI). The indicator is designed for low timeframes and aims to identify potential trend reversals in the market.

The indicator calculates the buy and sell signals based on the CCI and the SMAs. When the CCI is above the SMAs, a buy signal is generated. When the CCI is below the SMAs, a sell signal is generated. The indicator also provides alert signals to notify the user of potential entry or exit points.

Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in the product. To find the official developer of this product, please use MQL5.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-buy-sell-signal-low-tf-mt4-forex-trend-indicator/).
