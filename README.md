# Portfolio Optimization Beyond Mean-Variance: Incorporating Transaction Costs, Forecasts, and Tail Risk Control

In this project, we extended the classical Markovitz mean-variance portfolio optimization framework to incorporate practical considerations such as **transaction costs**, **return forecasts**, **fixed and piecewise-linear market frictions**, and **tail risk constraints**. Using real historical data (from May 6, 2024 to May 5, 2025), we implemented five increasingly sophisticated models in Julia using JuMP and Gurobi. Each model captured different layers of real-world complexity, from liquidity-aware rebalancing penalties to fixed operational costs and Value-at-Risk control.

Empirical results in Section 4 highlight the impact of these enhancements. Forecast-based models (e.g., Model 3.2) generated more responsive asset selections than static mean estimates, while incorporating transaction costs and operational consts led to **sparser, more stable portfolios** that avoided excessive turnover. Fixed and nonlinear costs further refined reallocation decisions by discouraging unnecessary trades, and the VaR constraint offered **explicit downside protection**. In our four-week backtest, all models **outperformed the DJIA benchmark**, with Models 3.3 and 3.5 achieving the strongest cumulative returns, while Model 3.2 provided the smoothest performance profile.

While our models provide a richer and more realistic optimization approach, we also acknowledge limitations—most notably the assumption of normal returns and the single-period horizon. In Section 5, we proposed several extensions, such as **multi-period optimization**, **Conditional Value-at-Risk**, and **sector or ESG constraints**, which would enhance realism and further align the model with institutional investment practices.

Overall, this project demonstrates how advanced optimization tools can bridge theory and practice, yielding actionable insights and robust investment decisions in dynamic market environments.

The content is Copyright &copy; 2025, Peter Xingyu Zhao & Qiushi Lu.

This workbook is provided under a Creative Commons Attribution-NonCommercial 4.0 International license. See https://creativecommons.org/licenses/by-nc/4.0/ for the explanation and https://creativecommons.org/licenses/by-nc/4.0/legalcode for the license itself.
