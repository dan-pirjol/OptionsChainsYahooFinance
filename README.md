This repository contains R code for downloading option chains from Yahoo Finance. 

The code *loadOptionChainsOMFormat.R* downloads the option chains for a given ticker and saves them to a .csv file in Option Metrics format, see below.

<img width="790" height="137" alt="OMformat" src="https://github.com/user-attachments/assets/ab3a4ad7-03c5-4ab0-82d5-c184a223d9f3" />

The code keeps only options without any NA in any row.

The function *getForward()* computes the forward prices as the solution to the equation C(K) = P(K) using mid-prices. 
The code *listOptionPrices.R* contains sample usage of this function.

**Example: SPY 9-Feb-2026**

The option chains for SPY were downloaded after 16:00EST and are in the file *SPY_options_9Feb2026.csv*

The forwards computed from option prices are in *SPY_forwards_9Feb2026.xlsx*. 

They can be compared against the Bloomberg forwards which can be seen in the OVDV screen below.

![SPY9Feb26](https://github.com/user-attachments/assets/f4eecef8-0d21-4caa-a9f6-147844fa3373)

The comparison is shown in the plot below. The two results agree reasonably well for maturities up to 9 months.

<img width="606" height="437" alt="SPYforwards-9Feb2026" src="https://github.com/user-attachments/assets/04d85a2d-93e9-44fd-b33e-4fda33108850" />
