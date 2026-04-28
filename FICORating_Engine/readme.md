
### FICO Quantization & Rating Engine
Python-based optimization tool for mapping continuous credit scores into discrete risk buckets. The engine utilizes Dynamic Programming to maximize the Log-Likelihood of default distributions, ensuring that each credit rating maintains maximum statistical significance for mortgage default prediction.

**Graph Displays Step-Function (Bucket) logic and Default Density Extrapolation**

-

**Optimization Logic**

Quantization (Rating): Groups 300–850 FICO scores into 10 distinct ratings (e.g., Rating 1 to 10).

Boundary Selection: Maximizes the statistical "distance" between buckets to ensure each rating reflects a significantly different default risk.

-

**The Math**

If $LogLikelihood_{Current} < LogLikelihood_{Optimized}$,  ----  then (update bucket boundaries).

Objective Function: $\sum_{i=1}^{m} [k_i \ln(p_i) + (n_i - k_i) \ln(1 - p_i)]$

Dynamic Programming: Iteratively solves for the optimal split points $b_i$ across the FICO range to reach a global maximum.

Rating Mapping: $Rating = f(FICO)$, where Rating 1 is assigned to the highest FICO scores (lowest risk).
