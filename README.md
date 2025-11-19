# Trader_Behavior_Insights

**Objective:** Explore relationships between Bitcoin market sentiment (Fear/Greed) and trader performance using Hyperliquid historical trade data to surface insights for smarter trading strategies.

**Approach:** Cleaned and merged trade and sentiment datasets by trade date; computed per-trade returns and per-trader aggregates; performed EDA, statistical tests, and a simple predictive model to measure sentiment's explanatory power.

**Top insights (example placeholders — replace with your computed numbers):**
- "Trades executed on Fear days had X% lower median returns compared to Greed days."
- "High-leverage trades during Fear periods had an elevated probability of negative PnL (win rate dropped by Y percentage points)."
- "A RandomForest model achieved AUC=B when predicting profitable trades using features: leverage, notional, hour_of_day, and sentiment_score — sentiment contributed C% to feature importance."

**Actionable recommendations:**
1. Consider reducing position sizes or leverage when rolling average sentiment indicates Fear.
2. Implement guardrails: max_leverage cap and smaller notional sizing during high-volatility periods.
3. Monitor sentiment shifts using a 7-day rolling average rather than daily spikes.

**Limitations & next steps:**
- Data sampling bias may exist (dominant accounts may skew results). Use per-account normalization or median-based metrics.
- Consider more advanced causal analysis (Granger causality) and intraday sentiment alignment if intraday sentiment becomes available.

