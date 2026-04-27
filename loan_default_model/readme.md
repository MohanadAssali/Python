
### Natural Gas Forward Curve Tool
Python-based risk assessment engine for retail loan portfolios. The tool utilizes Logistic Regression to transform multi-dimensional borrower data—including credit history, debt leverage, and employment stability—into a calibrated Probability of Default (PD) and Expected Loss (EL) framework.

**Graph Displays Sigmoid (S-Curve) Behavior and Risk Sensitivity Thresholds**

-

**Trade Logic**

Default (Loss): Occurs when borrower financial indicators (FICO, DTI) breach the model's classification boundary.

Recovery (Gain): Represents the 10% Recovery Rate—the capital the bank expects to recoup through asset liquidation or collections.

-

**The Math**

If $PD \times LGD \times EAD > Provisioning\_Limit$,  ----  then (High Risk / Capital Charge Required).

