# MT5 to Discord Signal Provider Utility

This code is a utility that allows users to send trading signals from MetaTrader 5 (MT5) to a Discord server. It provides a customizable order details class and a signal sender class to send the order details to the specified Discord server.

## OrderDetails Class
The `OrderDetails` class is used to store and retrieve information about a trading order. It has the following properties:

- `symbol`: The symbol of the trading instrument.
- `volume`: The volume of the trading order.
- `price`: The price at which the trading order should be executed.
- `type`: The type of the trading order (e.g., buy or sell).
- `stopLoss`: The stop loss level for the trading order.
- `takeProfit`: The take profit level for the trading order.

The class also provides getter and setter methods to access and modify the order details.

## SignalSender Class
The `SignalSender` class is responsible for sending the trading signals to the specified Discord server. It has a constructor that takes the Discord server name as a parameter. The `sendSignal` method takes an `OrderDetails` object as an argument and sends the order details to the Discord server.

## Main Program
The `OnStart` function is the entry point of the program. It creates an `OrderDetails` object with the specified order details (symbol, volume, price, type, stop loss, and take profit). It then creates a `SignalSender` object with the name of the Discord server. Finally, it calls the `sendSignal` method of the `SignalSender` object to send the order details to the Discord server. The program execution is completed by printing a success message.

Please note that Forex Robot Easy is not the official developer of this product. We are only providing the sample code that can work as described in this product. For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/mt5-to-discord-signal-provider-review-enhance-forex-trading-with-no-dll-utility/). To find the official developer of this product, please use MQL5.
