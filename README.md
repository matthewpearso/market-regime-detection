market-regime-detection project:
│
├── 📁 data/                         # Raw and processed data
│   ├── sp500.csv
│   ├── vix.csv
│   └── features.csv
│
├── 📁 notebooks/                   # Jupyter notebooks for exploration
│   ├── data_organization.ipynb
│   ├── regime_detection.ipynb
│   ├── strategy_design.ipynb
│   └── backtesting_evaluation.ipynb
│
├── 📁 src/                         # Core codebase
│   ├── __init__.py
│   ├── data_loader.py             # Load, process, and calculate new data
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
