### Natural Gas Forward Curve Tool
Python-based valuation engine for physical Natural Gas storage contracts. The tool extrapolates sparse monthly market data into a granular, daily forward curve by accounting for long-term price trends and monthly seasonality.

**Graph Displays Sine/Cosine logic/Staircase Behavior and Forward Extrapolation**

## Trade Logic
Injection (Buy): Usually happens in Summer (low demand).

Withdrawal (Sell): Usually happens in Winter (high demand).

The Math: 

If $Price_{Winter} - Price_{Summer} > Storage\_Costs$,  ----  then (profitable trade).


<img width="798" height="436" alt="5e79d82691ca9318992bf64fda14ceb0" src="https://github.com/user-attachments/assets/1c389fed-9a10-4461-9826-f3ba076590b6" />
