# RL-Ensemble-Trading

🔁 RL Ensemble Trading on NIFTY50 using A2C, PPO, DDPG, TD3, SAC. Includes portfolio optimization via MVO and dynamic LSTM/Transformer-based weighting. Benchmarked against NIFTY. Built fully in Python with interpretable metrics and strategy visualization.

## Overview

This repository implements a robust reinforcement learning (RL) ensemble trading system focused on the NIFTY50 index. It leverages multiple advanced RL algorithms—**A2C, PPO, DDPG, TD3, SAC**—and combines their outputs using portfolio optimization and dynamic deep-learning-based weighting strategies (LSTM and Transformer). The project is benchmarked against the NIFTY index and provides interpretable evaluation metrics and visualizations.

## Features

- **Ensemble of RL Agents:** Simultaneous use of A2C, PPO, DDPG, TD3, and SAC for trading.
- **Portfolio Optimization:** Uses Mean-Variance Optimization (MVO) and dynamic weight allocation via LSTM/Transformer models.
- **Benchmarked Performance:** Evaluates and compares RL ensemble against NIFTY index and individual agent strategies.
- **Interpretable Metrics & Visualization:** Returns, risk metrics, and strategy visualizations for actionable insights.
- **Python Ecosystem:** Built on top of [FinRL](https://github.com/AI4Finance-Foundation/FinRL), [Stable Baselines 3](https://stable-baselines3.readthedocs.io/en/master/), Torch, and related libraries.

## Main Components

- `1_Data.ipynb`: Data collection and preprocessing for NIFTY50 stocks.
- `2_Train.ipynb`: Training RL agents, portfolio optimization, and dynamic weighting.
- **Dynamic Weighting Features:**
  - LSTM & Transformer models for return prediction.
  - Automatic feature engineering from strategy returns.
  - Risk-adjusted weight calculation and real-time portfolio rebalancing.
  - Comprehensive performance analysis.
- **Integration:** Utilizes FinRL and ElegantRL for DRL agents; Ray RLlib is also supported.

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook/Lab

### Installation

Install core dependencies:
```bash
pip install git+https://github.com/AI4Finance-Foundation/FinRL.git
pip install torch scikit-learn seaborn
```
The notebooks will also handle the installation of certain dependencies (e.g., ElegantRL, Ray RLlib) as required.

### Additional Requirements

Some commonly used packages (installed automatically or via requirements):
- `finrl`
- `elegantrl @ git+https://github.com/AI4Finance-Foundation/ElegantRL.git`
- `ray`
- `pyportfolioopt`
- `cvxpy`
- `torch`
- `scikit-learn`
- `seaborn`
- `gymnasium`

### Usage

1. **Data Preparation:**  
   Open and execute `1_Data.ipynb` to fetch and preprocess NIFTY50 data.

2. **Training & Optimization:**  
   Run `2_Train.ipynb` to:
   - Train DRL agents on the NIFTY50 data.
   - Perform ensemble weighting (MVO, LSTM, Transformer).

3. **Backtesting & Analysis:**  
   Execute `3_Backtest.ipynb` to:
   - Backtest and analyze strategy performance.
   - Visualize and compare ensemble vs. individual agent and NIFTY benchmarks.

4. **Dynamic Weighting & Evaluation:**  
   - Analyze weight evolution and metrics.

### Customization

- Users can experiment with different RL libraries, such as [ElegantRL](https://github.com/AI4Finance-Foundation/ElegantRL) or [Ray RLlib](https://github.com/ray-project/ray).
- Hyperparameters and model architectures can be modified in the notebooks.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- [FinRL](https://github.com/AI4Finance-Foundation/FinRL)
- [Stable Baselines 3](https://stable-baselines3.readthedocs.io/en/master/)
- [ElegantRL](https://github.com/AI4Finance-Foundation/ElegantRL)
- [Ray RLlib](https://github.com/ray-project/ray)

## Contact

For questions or contributions, please open an issue or contact [RonitKhanna333](https://github.com/RonitKhanna333).

---
*This repository provides a state-of-the-art, interpretable RL ensemble framework for financial trading research and experimentation on the NIFTY50 index.*
