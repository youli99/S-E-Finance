1. Filter
Keep all the firms marked as "Eur" in "Static.xlsx"
Keep all the firms existing in "GScore.xlsx"
Take the intersection

2. Data cleaning

1) Return Index (monthly) dataset:
Calculate the monthly simple returns
Replace the outliers (>100 & <-100) of the average of its previous and next value
Fill NaN at the beginning/end with the average of the available samples over the row
Linear interpolation for the missing value at the middle 

2) Market Value (monthly) dataset:
Considering market dynamics, no treatment for possible outliers
Fill NaN at the beginning/end with the average of the available samples over the row
Linear interpolation for the missing value at the middle 

Note: use the same sample for Q1-4.

3. Calculations
Annualized average return: average of the monthly returns over the sample period * 12
Annualized volatility: standard deviation of the monthly returns * sqrt(12)
Annualized Sharpe ratio: (average of the excess returns * 12) / (standard deviation of the excess returns * sqrt(12))


