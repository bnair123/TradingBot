# Project overview and brainstorming

## Core questions
### System architecture
- Backtesting enginr
- Trading scorer and nalysis
- Baseline trading bot
- data pipeline
- Execution engine
- Rt or batch?

### Machine Learning Approach
- Model Selection: Which ML algorithms to compare? 
  - Supervised learning (classification/regression)?
  - Reinforcement learning?
  - Time series specific models (LSTM, Transformers)?
  - Traditional ML (Random Forest, XGBoost)?

- Should we run multiple model types in parallel? 
  - Combine different models? COmpare models?

- What features should each model use?

- Technical indicators (RSI, MACD, Moving Averages)?
- Price/volume data?
- Market sentiment?
- Fundamental data?
- Do all models get sam features or custom per model? 
  - How to handle feature selection/importance?

Model Output Design

 - Simple approach: Buy/Hold/Sell + confidence score
 - Complex approach: Position sizing, multiple assets, portfolio allocation
 - Discrete actions vs continuous predictions?
 - Single prediction vs prediction distribution?

## Risk managment
- Do we add any risk management for this exploration?
  - If yes then what kind? Stop-loss, take-profit, position sizing?
  - If no, how do we ensure the models don't take excessive risk?
  - Do we make a seperate risk management module? or integrate into models?

## Data
- What data sources to use?
  - Historical price data (Yahoo Finance, Alpha Vantage, etc.)
  - Fundamental data (financial statements, ratios)
  - Alternative data (news sentiment, social media)
- Data frequency: Daily, intraday, tick data?
- How much data is needed?
- Cleaning the data necessary?
- If supervised learning how to label sufficient data?
- How to avoid overfitting?
- Train and test strategy

## Evaluation
- What metrics to use for evaluation?
  - Standard financial metrics (CAGR, Sharpe Ratio, Max Drawdown)
  - Compare vs baseline strat, buy and hold and random trading

## Techncials
- Programming language and libs
- Data handling (store in a db or flat files? or directly from APIs?)
- Enviroment to run it? Ie docker for continous trades?
  
## Other questions
- Fix to certain assets or multiple assets?
- Entire portfolio or single asset trading?
- Time horizon
- Transaction costs, slippage?