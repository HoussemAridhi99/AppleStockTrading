# 💹 Reinforcement Learning for Stock Trading

This project applies Reinforcement Learning (RL) techniques to create an agent that learns to trade stocks. It uses a Q-Learning approach on historical financial data to maximize profit through optimal trading actions.

## 🧠 Objective

To train an RL agent that can learn optimal trading strategies (Buy, Hold, Sell) for a selected stock based on historical price data and technical indicators.

## 🛠️ Technologies & Libraries

- Python
- Pandas, NumPy
- Matplotlib
- Gym
- Scikit-learn
- Yahoo Finance (via `yfinance`)
- `stable-baselines3` *(optional, not in current version)*

## 📊 Dataset

- Source: Yahoo Finance
- Data features: `Open`, `High`, `Low`, `Close`, `Volume`, plus technical indicators (e.g., Moving Averages)

## 🔁 Workflow

1. **Data Collection** using `yfinance`
2. **Feature Engineering** with technical indicators
3. **Environment Setup** (Custom Gym environment)
4. **Q-Learning Agent**:
   - States: combinations of indicators and holdings
   - Actions: Buy, Sell, Hold
   - Rewards: Portfolio value change
5. **Training Loop** with Q-Table updates
6. **Evaluation & Visualization** of trading performance

## 🤖 Reinforcement Learning Details

- **Algorithm**: Tabular Q-Learning
- **Actions**: 
  - `0`: Hold  
  - `1`: Buy  
  - `2`: Sell
- **State**: Discretized based on market indicators and inventory status
- **Reward**: Change in total portfolio value after each step

## 📈 Performance & Visualization

- Portfolio value vs. time
- Buy/Sell signals on stock price chart
- Q-Table heatmaps (optional)

