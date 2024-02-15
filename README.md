# Gann Square of 9 Indicator ReadMe File

This ReadMe file provides an overview of the Gann Square of 9 Indicator for Forex Trading Environment. The code provided is a sample implementation of the indicator and is not the official product developed by Forex Robot Easy.

## Indicator Description

The Gann Square of 9 Indicator is a tool used in forex trading to identify potential support and resistance levels based on the principles of Gann theory. It calculates price levels and time levels using a square size parameter and the number of levels to display.

## Indicator Parameters

The following parameters can be customized when using the Gann Square of 9 Indicator:

- `squareSize`: The square size of the Gann Square of 9.
- `levels`: The number of levels to display.

## Indicator Variables

The indicator uses the following variables:

- `priceLevels[]`: An array to store the calculated price levels.
- `timeLevels[]`: An array to store the calculated time levels.

## Indicator Data

The `OnInit()` function initializes the indicator by resizing the `priceLevels` and `timeLevels` arrays and calculating the price and time levels based on the provided parameters.

The `CalculatePriceLevel()` function calculates the price level for a given level using the square root of the level multiplied by the square size parameter.

The `NormalizePrice()` function normalizes the calculated price to the appropriate number of digits.

The `CalculateTimeLevel()` function calculates the time level for a given level based on the current time and the square size parameter.

## Trading Functions

The following functions can be used to enter and exit trades based on the calculated price and time levels:

- `EnterTrade(double price, datetime time)`: Add your logic for entering a trade here.
- `ExitTrade(double price, datetime time)`: Add your logic for exiting a trade here.

## Indicator Calculation

The `OnCalculate()` function is called to calculate the indicator for each bar in the chart. It iterates through the price and time levels and checks if the current price and time are greater than or equal to the level price and time. If the condition is met, the `EnterTrade()` and `ExitTrade()` functions are called.

## Indicator Deinitialization

The `OnDeinit()` function is called when the indicator is removed from the chart. You can add your deinitialization logic here.

## Product Description

This code provides a sample implementation of the Gann Square of 9 Indicator for Forex Trading. It calculates price and time levels based on the provided parameters and allows for custom trading logic to be added.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in the product. For detailed reviews and trading results of the official product, please visit [Forex Robot Easy - Gann Square of 9 Review](https://forexroboteasy.com/forex-robot-review/gann-square-of-9-review-accurate-forex-trading-tool/). To find the official developer of this product, please refer to MQL5.
