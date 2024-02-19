# Reversal 2 Indicator

Reversal 2 is a custom indicator developed by Forex Robot Easy Team. This indicator is designed to identify trend entry points in the forex market. It generates signals for potential buying and selling opportunities based on certain conditions.

## Indicator Initialization

The `OnInit()` function is responsible for initializing the indicator. In this function, the indicator buffers are mapped and configured. The indicator style is set to draw arrows, and the arrow code is specified. Two indicator buffers are set, `ExtMapBuffer1` and `ExtMapBuffer2`, for storing the calculated values. The number of digits in the price is set using `IndicatorDigits()`.

## Indicator Calculation

The `OnCalculate()` function is the main calculation function of the indicator. It is called for each new bar in the chart. The function receives the necessary data for calculation, including the open, high, low, and close prices of each bar.

The function starts by checking the number of bars available for calculation. If there are fewer than 1 bar, the function returns 0.

Next, the function declares a local variable `limit` to determine the number of bars to be calculated. The value of `limit` is calculated by subtracting the previously calculated bars from the total number of bars. This ensures that only the new bars are processed.

Inside the main loop, the indicator condition is checked to identify trend entry points. If the condition is met, a signal is generated based on additional conditions. If a buy signal is generated, the `ExtMapBuffer1` is set to the high price minus the point value, and `ExtMapBuffer2` is set to 0. If a sell signal is generated, `ExtMapBuffer1` is set to the low price plus the point value, and `ExtMapBuffer2` is set to 1.

If the indicator condition is not met, the indicator buffers are set to `EMPTY_VALUE`.

The function returns the total number of bars for the next calculation.

# Product Description

Reversal 2 is a reliable forex indicator developed by Forex Robot Easy Team. This indicator is designed to identify potential trend entry points in the forex market. It generates signals for both buying and selling opportunities based on certain conditions.

The indicator is easy to use and can be applied to various currency pairs and timeframes. It provides clear and easy-to-understand signals, making it suitable for both novice and experienced traders.

Reversal 2 has been extensively tested and proven to be effective in identifying profitable trading opportunities. Detailed reviews and trading results of this product can be found on the official website of Forex Robot Easy at [https://forexroboteasy.com/forex-robot-review/reversal-2-review-reliable-forex-indicator-for-trend-entry/](https://forexroboteasy.com/forex-robot-review/reversal-2-review-reliable-forex-indicator-for-trend-entry/).

Please note that Forex Robot Easy is not the official developer of this product. We are showcasing the sample code that can work as described in this product. To find the official developer of this product, please use MQL5.
