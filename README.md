# Autonomous Crypto Trading Bot
Run `make build`, then `make play` to view the autonomous trading bot in action. 
## Output at Termination of Program
![Trading Bot Output](https://i.ibb.co/D9sVhT3/gries.png)
<br> Our algorithm made a profit of $27,863.78, which generates $24,478.54 more than if the trader held their positions for the duration of the trading period.
## Introduction
This is a crypto trader that trades on the price of the cryptocurrency Etheruem, aka ETH. We make our decision based on three different factors. At the very core, the decision algorithm’s sensitivity to each of these factors is adjustable with hyperparameters. <br><br>
First, we employ the calculations of four different indicators: MACD, RSI, OBV, and Stochastic Oscillator. Each of these indicators evaluates on a different aspect of the coin, such as it's historical moving average or volume. <br><br>
Second, our algorithm compares the price of the current day to every historical trendline to predict the price’s future direction. It uses the frequency of critical points to update the relative "strength" of a trendline as means of support and resistance. <br><br>
Finally, our algorithm creates grid lines proportional to the price of the coin, and giving a marginal bound of 30% on each side. When the price of the coin increases past a grid line (i.e. passes a red grid line), a signal to buy will be sent. When the price of the coin decreases below a grid line (i.e. passes a green grid line), a signal to sell will be sent. <br><br>
We allow you, the user, to control this last part of our trading algorithm, but do not fret! Our algorithm will automatically adjust the bounds for you if they are too far from the price of the coin. 
