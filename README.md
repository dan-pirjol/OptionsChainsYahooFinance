This repository contains R code for downloading option chains from Yahoo Finance and saving them as csv file in Option Metrics format, see below.

<img width="790" height="137" alt="OMformat" src="https://github.com/user-attachments/assets/ab3a4ad7-03c5-4ab0-82d5-c184a223d9f3" />

The code keeps only options without any NA in any column.

The code listOptionPrices.R computes the forward prices as the solution to the equation C(K) = P(K). 

**Example: SPY 9-Feb-2026**

The forwards can be compared against Bloomberg forwards. 


