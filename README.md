README.md

# DaneTrades.mq5

This code is a sample trading robot written in MQL5, the programming language used for creating Expert Advisors (EAs) in the MetaTrader 5 platform. 

The DaneTrades robot is designed to automate trading operations based on predefined conditions. It includes risk management parameters, breakeven stop loss, trailing stop loss, max daily loss prevention, and overtrading prevention.

## Risk Management Parameters

- Risk Calculation: Choose between calculating lot size based on a percentage of the account balance or a fixed amount.
- Risk Percentage: The percentage of the account balance to risk per trade.
- Risk Fixed Amount: The fixed amount to risk per trade.
- Use Fixed Lots: Whether to use a fixed lot size or calculate it based on the risk management settings.

## Breakeven Stop Loss Parameters

- Breakeven Mode: Choose between setting the breakeven stop loss based on pips or price.
- Breakeven Pips: The number of pips to set the breakeven stop loss.
- Breakeven Price: The price level to set the breakeven stop loss.

## Trailing Stop Loss Parameters

- Trailing Stop Pips: The number of pips to trail the stop loss.

## Max Daily Loss Parameters

- Max Daily Loss Mode: Choose between limiting the maximum daily loss based on a percentage of the account balance or a fixed amount.
- Max Daily Loss Percentage: The maximum percentage of the account balance to lose in a day.
- Max Daily Loss Amount: The maximum amount to lose in a day.
- Total Daily Profit: The total profit or loss made during the day.

## Overtrading Prevention Parameters

- Min Time Between Trades: The minimum time in minutes between opening trades.
- Last Trade Time: The time of the last trade opened.

## Expert Initialization Function

The `OnInit()` function is called during the initialization of the Expert Advisor. This is where necessary variables and settings are initialized.

## Expert Deinitialization Function

The `OnDeinit()` function is called during the deinitialization of the Expert Advisor. This is where any necessary cleanup can be performed.

## Expert Start Function

The `OnTick()` function is called on each tick of the market. This is where the conditions to open a trade are checked. If the conditions are met, the trade is opened, and the breakeven stop loss, trailing stop loss, daily profit update, and max daily loss checks are performed. The last trade time is also updated.

## Additional Functions

- `CanOpenTrade()`: Checks if a trade can be opened based on the trade opening conditions and overtrading prevention.
- `CalculateLotSize()`: Calculates the lot size based on the risk management settings.
- `SetBreakevenStopLossByPips()`: Sets the breakeven stop loss based on pips.
- `SetBreakevenStopLossByPrice()`: Sets the breakeven stop loss based on price.
- `SetTrailingStopLoss()`: Sets the trailing stop loss based on pips.
- `UpdateDailyProfit()`: Updates the daily profit.
- `CloseAllTrades()`: Closes all open trades.

## Product Description

DaneTrades is an automated trading robot developed by Forex Robot Easy Team. This sample code demonstrates the functionality of the DaneTrades EA, which is designed to automate trading operations in the MetaTrader 5 platform.

The DaneTrades robot includes various risk management parameters, such as the ability to calculate lot size based on a percentage of the account balance or a fixed amount. It also includes features like breakeven stop loss, trailing stop loss, max daily loss prevention, and overtrading prevention.

Please note that Forex Robot Easy is not the official developer of the DaneTrades product. We only provide this sample code to showcase how the product works based on the information available. For detailed reviews and trading results of the DaneTrades EA, please refer to the official developer or visit [Forex Robot Easy's review](https://forexroboteasy.com/forex-robot-review/trade-manager-mt4-danetrades-automated-forex-software-review/).

To find the official developer of the DaneTrades product or to obtain the complete and official version, please use the MQL5 platform.
