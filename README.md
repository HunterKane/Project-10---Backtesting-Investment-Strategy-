# Project-10---Backtesting-Investment-Strategy-

Backtesting Investment Strategy:
- Purpose of projet is to examine daily Close prices of stocks from 2010-01-01 to 2020-03-31 for DOW JONES. 

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
