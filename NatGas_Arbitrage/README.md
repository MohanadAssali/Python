
### Natural Gas Storage Valuation Prototype
Python-based valuation engine for physical Natural Gas storage contracts. This prototype builds upon the forward curve tool to calculate the total contract value by simulating multi-event trading strategies against physical facility constraints.

**Graph Displays Continuous forward curve extrapolation (Sine/Cosine logic), historical market snapshots, and the elimination of step-wise pricing for granular daily valuation.**

-

**The Math**

$$(Price_{Sell} - Price_{Buy}) \times Volume > Storage\_Costs + Movement\_Fees$$

-

**Trade Logic**

Injection (Buy): Occurs during price troughs (Summer/Low demand).

Withdrawal (Sell): Occurs during price peaks (Winter/High demand).

Safety Checks: Built-in logic to prevent exceeding Max Capacity or withdrawing more than the current Inventory.

-

**Test Case Result**

Contract Value: $451,238.80 (Calculated from 1M MMBtu summer-to-winter arbitrage).

<img width="457" height="358" alt="bca4d9828e490075cadbaa521bd4c27f" src="https://github.com/user-attachments/assets/777e96b0-ab55-4932-8795-f13904df6edb" />

