# Market Regime Adaptive Strategy Backtester

This project detects historical market regimes (e.g., bull, bear, sideways) using unsupervised learning and applies regime-specific trading strategies to optimize performance.

## 📈 Key Features
- Regime detection using K-Means and HMM
- Momentum and mean reversion trading strategies
- Adaptive strategy switching
- Backtesting and performance evaluation

## 🧪 Technologies Used
- Python (pandas, scikit-learn, hmmlearn, Backtrader)
- yFinance for historical data
- Matplotlib and Seaborn for visualization

## 🗂️ Folder Guide
- `notebooks/` – Step-by-step development
- `src/` – Modular codebase for reuse and testing
- `reports/` – Result plots and summary
- `dashboard/` – (Optional) Streamlit app

## 📊 Sample Results
![Cumulative Returns](reports/performance_summary.png)

## 🚀 Getting Started
```bash
pip install -r requirements.txt
python src/backtester.py

quant-regime-trader/
│
├── 📁 data/                         # Raw and processed data
│   ├── sp500.csv
│   ├── vix.csv
│   └── features.csv
│
├── 📁 notebooks/                   # Jupyter notebooks for exploration
│   ├── 01_data_download.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_regime_detection.ipynb
│   ├── 04_strategy_design.ipynb
│   └── 05_backtesting_evaluation.ipynb
│
├── 📁 src/                         # Core codebase
│   ├── __init__.py
│   ├── data_loader.py             # Load and process raw data
│   ├── features.py                # Feature engineering logic
│   ├── regime_model.py            # Clustering/HMM models
│   ├── strategy/                  # Trading strategy classes
│   │   ├── __init__.py
│   │   ├── momentum.py
│   │   ├── mean_reversion.py
│   │   └── adaptive_strategy.py   # Strategy switcher
│   ├── backtester.py              # Runs backtests using Backtrader
│   └── evaluation.py              # Sharpe, drawdown, plots, etc.
│
├── 📁 reports/                     # Visualizations and summary outputs
│   ├── performance_summary.png
│   └── regime_overlay_plot.png
│
├── 📁 dashboard/ (optional)       # Streamlit dashboard app
│   ├── app.py
│   └── requirements.txt
│
├── requirements.txt               # Python dependencies
├── README.md                      # Project overview and results
├── .gitignore                     # Files to ignore (e.g., .ipynb_checkpoints)
└── LICENSE                        # (Optional, e.g., MIT)
