# Next-Alpha: 7-Day Crypto Range Predictor
**🏆 Championship Winner | International Quant Challenge**

Next-Alpha is an award-winning quantitative forecasting system designed to predict the volatility and price ranges of major cryptocurrencies. This project was developed for the **International Quant Challenge**, where it secured a top-tier victory for its innovative approach to generating actionable "Alpha" in the volatile crypto market.

## 🌟 Achievement Highlights
- **1st Place Winner:** Recognized for superior predictive accuracy and robust model architecture.
- **Multiple Award-Winning Developer:** Part of a portfolio that secured **Top 3 at 2 other instances also**.
- **Institutional Grade Logic:** Engineered to handle real-world market noise for assets including **Arbitrum (ARB)**, **Chainlink (LINK)**, and **Ethereum (ETH)**.

## 📈 Strategic Overview
The "Next-Alpha" engine moves beyond simple price guessing. It utilizes a hybrid statistical approach to predict **Price Range Categories**. This allows traders and automated systems to identify high-probability "safety zones" for liquidity provision and options trading.

### Key Technical Features
- **Live Market Integration:** Seamless data pipeline using the CoinGecko API for real-time model refreshing.
- **Hybrid Time-Series Architecture:** Combines **FBProphet's** additive modeling with **SARIMAX** to account for both cyclical trends and sudden market shocks.
- **Range Categorization:** Implements a proprietary labeling logic (e.g., `pr_1_1_1_2`) to map numerical forecasts to executable trading ranges.
- **Volatility Scaling:** Uses `StandardScaler` and rolling variance to normalize inputs across assets with different market caps.

## 🛠️ Tech Stack
- **Languages:** Python 3.x
- **Time-Series Analysis:** `Prophet`, `Statsmodels` (SARIMAX)
- **Data Science:** `Pandas`, `NumPy`, `Scikit-learn`
- **Visualization:** `Matplotlib` (Forecasting vs. Backtest overlays)

## 📊 Methodology
1. **Dynamic Ingestion:** Extracts 365+ days of historical tick data to train on diverse market regimes.
2. **Decomposition:** Breaks down price action into Trend, Seasonality (Weekly/Monthly), and Residual Noise.
3. **Parameter Optimization:** Systematic grid search for $(p, d, q)$ parameters to maximize the Log-Likelihood of the model.
4. **Range Projection:** Outputs a 7-day forward-looking window with upper and lower confidence bounds.

## 🚀 Setup & Execution

### Installation
```bash
pip install pandas numpy matplotlib requests prophet statsmodels
