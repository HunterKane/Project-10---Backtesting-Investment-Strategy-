# Project-10---Backtesting-Investment-Strategy-

Backtesting Investment Strategy:
- Purpose of this project is to examine daily Close prices of stocks from 2010-01-01 to 2020-03-31 from the DOW JONES constituents. 

__Method__:
- Create active strategies that outperform a passive buy and hold strategy for the Dow Jones Index.
- BAC testing / Further testing

__Backtesting a simple Momentu Strategy__

__Positions__:
- +1: Investing in DJl(long position)
- -1: Short Selling DJl(short position)
- 0: No position(neutral)

__Strategy__:
- Buy and Hold(Basic Strategy - passive): Initially Investing into DJl and do nothing(Position +1 on any given day)
- Simple Momentum(active strategy to be tested):
- a)Investing(+1) into DJl tomorrow if today's returns were positive
- b)Short Selling(-1) into DJl tomrrow if today's returns were negative


__Conclusion of Basic Strategy__:

- From an emulated basses we have a return of - 5%
- DOW JONES return 0.07% per year

__Key Finding__:
Our momentum strategy underperforms the basic buy and hold strategy. Not a beneficial long term strategy.


__Backtesting a simple Contrarian Strategy__:

- Buy and Hold(Basic Strategy): Initially Investing into the DJI and do nothing(Position: +1 on all days)
- Simple Contrarian(Strategy to be tested):
- Short selling(-1) DJI tomorrow if today's return was positive
- Investing(+1)into DJI tomorrow if today's return was negative


__More Complex Strategies & Backtesting vs. Fitting__:
- Try to find a strategy that outperforms our buy and hold strategy
- **Note: Backtesting is performed on historical data available / Fitting follows the system's logic in a live market

__Conclusion from Fitting testing__:

- Even if a strategy seems to outperform the basic Strategy, the following issues need to be considered/analyzed as well:
- Backtesting Vs. Fitting -> Was the strategy fitted and optimized on historical data? Forward testing is required
- Transaction Costs -> Chaning positions trigger cost. Include costs.
- Tax efffects -> Changing positions can trigger tax payments. Include tax.


__Simple Moving Averages (Crossovers) Strategy implemented to see if it outperforms or overperforms the Buy and Hold Strategy__.

- Buy and Hold(basic strategy): Initially Investing in DJI and do nothing (Position: +1 on all days) SMA Crossover(Momentum)(Strategy to be tested):
- a) Investing(+1): SMA50 > SMA200
- b) Short Selling(-1):SMA50 < SMA200 

__Final Conclusions from the data__:
- Positions change when both curves cross paths. From -1 to +1. When SMA50 is greater = +1 / When SMA50 is less than = -1
- Our strategy underperforms over the long term.
- No evidence shows that our simple moving average crossover momentum strategy over or outperforms the Buy and Hold strategy.
- Our strategy underperforms and we should not rely upon simple moving average strategies.
