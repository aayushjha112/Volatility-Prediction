# Volatility-Prediction
Key Features: <br>
Stock market variables: Parent Indices Data (NIFTY 50, NIFTY COMMODITIES, NIFTY INFRASTRUCTURE). <br>
Exogenous variables: USD INR Exchange Rate, Interest Rate (Repo Rate), Crude Oil Prices, FPI Data. <br>
Feature Engineering to create extra variables such as EMA, RSI, Log Returns, Price Change, Volume Ratio, Volatility. <br>
Multicollinearity Check: Correlation Matrix & Variance Inflation Factor (VIF). <br>
Time series train-test split (80:20). <br>
Used ARMAX to model log returns and checked ACF for seasonality and order. <br>
Tried all possible combinations till order (3,0,3). <br>
Ran LLR Test, checked AIC/BIC, resemblance of residuals to white noise to conclude ARMAX (1,0,1) as best. <br>
Ran GARCH on residuals to capture volatility clustering and checked ACF for order. <br>
Tried all possible combinations till order (3,3). <br>
Checked AIC/BIC, significance of higher order coefficient, resemblance of residuals to white noise to conclude GARCH (1,1) as best. <br>
Conducted multi-step and rolling 1-step forecast.
