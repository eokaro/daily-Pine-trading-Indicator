# RSI + EMA + Liquidity Sweep Strategy

This is a TradingView Pine Script strategy combining **RSI**, **EMA**, and **Liquidity Sweep** indicators to generate buy and sell signals for traders. The strategy utilizes the **RSI** for momentum analysis, **EMA** for trend confirmation, and **Liquidity Sweep** to capture significant market reversals.

## Features
- **RSI (Relative Strength Index)** to identify overbought and oversold conditions.
- **EMA (Exponential Moving Average)** to determine trend direction.
- **Liquidity Sweep** to identify sharp reversals, especially when liquidity is swept at critical price levels.
- **Backtesting Capability**: Use the initial capital of $10,000 to test performance over historical data.
- **Customizable Parameters**: Easy-to-adjust inputs for RSI period, EMA period, and liquidity sweep factors.

## Usage

### 1. Setup on TradingView:
1. Open **TradingView** and go to the **Pine Script Editor**.
2. Paste the provided Pine Script code into the editor.
3. Add the script to your chart.
4. Modify parameters as needed (RSI period, EMA period, etc.).
5. Set up alerts for automated signal notifications.

### 2. Strategy Parameters:
- **RSI Period**: Sets the period for the RSI indicator (default: 14).
- **Overbought Level**: The RSI value that triggers a sell signal (default: 70).
- **Oversold Level**: The RSI value that triggers a buy signal (default: 30).
- **EMA Period**: Period for calculating the EMA (default: 50).
- **Liquidity Lookback**: Defines how many bars to look back for the liquidity sweep logic (default: 10).
- **Sweep Factor**: The threshold percentage of the bar range used for liquidity sweep conditions (default: 0.7).

### Example:

- **Long Position**: Triggered when the RSI is below the oversold level, the price is above the EMA, or a bullish liquidity sweep is detected.
- **Exit Position**: Triggered when RSI is above the overbought level, or a bearish liquidity sweep is detected.

## Backtesting Results

Backtest the strategy using historical data on TradingView to analyze performance and tweak the parameters for your trading needs. See the **backtest_results/** folder for a summary of backtest results.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to fork the project, suggest improvements, or submit pull requests. See the [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.


