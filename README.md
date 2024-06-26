# Algorithm Trading using Unsupervised Machine Learning 

This project involves developing an algorithmic trading strategy that leverages unsupervised learning techniques to select and optimize a portfolio of S&P 500 stocks. The strategy employs K-Means clustering to group stocks based on their features and technical indicators and uses portfolio optimization techniques to construct a high-performing portfolio. The effectiveness of the strategy is evaluated by comparing the portfolio's returns against the S&P 500 benchmark


Data Collection and Preprocessing
Data Sources: Gathered S&P 500 stock prices and Fama-French factor data using financial data APIs and libraries such as pandas_datareader.
Data Cleaning: Processed raw data to handle missing values, normalize features, and prepare for analysis.
Aggregation: Aggregated data on a monthly level to align with the trading strategy's time horizon.


Feature Engineering
Technical Indicators: Calculated various technical indicators, including moving averages (MA), relative strength index (RSI), and moving average convergence divergence (MACD).
Financial Metrics: Computed additional financial metrics such as trading volume and liquidity measures.
Monthly Aggregation: Aggregated features and metrics on a monthly basis to facilitate consistent analysis.


Return Calculation
Monthly Returns: Analyzed monthly returns for each stock across different time horizons (like  1-month, 3-month, and 6-month returns).
Performance Metrics: Calculated performance metrics to assess stock returns and volatility.


Factor Analysis
Fama-French Factors: Retrieved Fama-French 5-factor data to account for market, size, value, profitability, and investment factors.
Rolling Betas: Computed rolling factor betas for each stock to understand its sensitivity to market factors over time.


Clustering Analysis
K-Means Clustering: Applied K-Means clustering algorithm monthly to group stocks based on their calculated features and indicators.
Cluster Evaluation: Evaluated cluster quality and adjusted parameters to ensure meaningful grouping of stocks.


Portfolio Optimization
Efficient Frontier: Constructed portfolios using Efficient Frontier principles to optimize the risk-return profile.
Max Sharpe Ratio: Utilized Max Sharpe Ratio optimization to select the best-performing portfolio from the clusters' assets.
Asset Selection: Based on the clusters, selected a diverse set of assets to enhance portfolio robustness and performance.


Performance Evaluation
Visualization: Visualized portfolio returns using various plotting techniques to provide clear insights into performance trends.
Benchmark Comparison: Compared the constructed portfolio's returns against the S&P 500 benchmark to evaluate the strategy's effectiveness.


Performance Metrics: Assessed key performance metrics such as Sharpe ratio, alpha, and beta to quantify the strategy's success.
