# Multi-Factor Equity Investment Model

A quantitative equity investment framework that evaluates stocks using multiple financial factors, ranks investment opportunities, and constructs portfolios based on systematic investment signals.

The project explores how factor-based investing can be used to identify potentially attractive equities, optimize portfolio allocations, and evaluate investment performance through historical backtesting.

## Project Overview

Traditional investment strategies often rely on individual financial metrics or subjective stock selection. This project combines multiple quantitative factors into a systematic stock-selection and portfolio-construction framework.

The model focuses on four established equity investment factors:

- **Value:** Identifies potentially undervalued stocks using valuation metrics.
- **Momentum:** Evaluates historical price performance to identify prevailing market trends.
- **Quality:** Assesses company fundamentals and financial strength.
- **Low Volatility:** Identifies stocks with relatively lower historical price fluctuations.

These factors are combined to generate stock rankings and evaluate portfolio performance.

## Key Features

- Multi-factor equity scoring and stock ranking.
- Value, momentum, quality, and low-volatility factor analysis.
- Information Coefficient (IC) analysis to evaluate factor effectiveness.
- Portfolio performance evaluation.
- Rolling-window portfolio analysis.
- Equity curve generation and visualization.
- Historical backtesting and performance measurement.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Statistical Analysis | Python statistical libraries |
| Visualization | Matplotlib |
| Financial Research | Quantitative factor analysis |
| Development | PyCharm, Git, GitHub |

## Project Structure

```text
equity-factor-investment-model/
│
├── factor_model.py
├── plot_results.py
├── rolling_analysis.py
├── plot_rolling.py
│
├── factor_scores.csv
├── ic_by_period.csv
├── ic_summary.csv
├── performance_metrics.csv
├── equity_curve.csv
├── rolling_equity_curve.csv
├── rolling_holdings_log.csv
├── rolling_performance_metrics.csv
│
├── equity_curve.png
├── rolling_analysis.png
│
├── requirements.txt
└── README.md
```

## Methodology

### 1. Factor Construction

The investment universe is evaluated using four equity factors: value, momentum, quality, and low volatility.

Individual factor signals are combined to produce composite stock scores and rankings.

### 2. Stock Ranking

Stocks are evaluated according to their factor scores to identify the strongest candidates under the selected investment framework.

### 3. Portfolio Backtesting

Historical portfolio performance is evaluated using the generated investment signals.

### 4. Information Coefficient Analysis

Information Coefficient analysis examines the relationship between factor rankings and subsequent stock returns to assess the predictive effectiveness of investment factors.

### 5. Rolling Performance Analysis

Rolling-window analysis evaluates portfolio performance across different historical periods rather than relying exclusively on one cumulative performance figure.

## Installation and Execution

Clone the repository:

```bash
git clone https://github.com/thedatajournal/equity-factor-investment-model.git
```

Navigate into the project:

```bash
cd equity-factor-investment-model
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the analysis scripts:

```bash
python factor_model.py
python plot_results.py
python rolling_analysis.py
python plot_rolling.py
```

## Results and Outputs

The project generates several outputs for quantitative evaluation:

- Factor scores and stock rankings.
- Information Coefficient summaries.
- Portfolio performance metrics.
- Cumulative equity curves.
- Rolling portfolio performance.
- Historical holdings information.

## Future Improvements

The following enhancements are planned to develop the framework into a more comprehensive quantitative investment research platform:

- Incorporate additional fundamental financial data.
- Implement sector-neutral factor scoring.
- Conduct factor Information Coefficient and stability analysis.
- Compare results against Fama-French factor models.
- Introduce mean-variance and risk-adjusted portfolio optimization.
- Incorporate transaction costs and realistic trading constraints.
- Evaluate performance against market benchmarks.
- Implement out-of-sample testing and robustness checks.

## Research Direction

The long-term objective is to develop a systematic equity investment framework that integrates financial fundamentals, statistical analysis, factor research, and portfolio optimization.

The project serves as a foundation for exploring quantitative equity research and systematic portfolio management.

## Acknowledgements

This project builds upon the original work by [henryletourneux/quant-equity-factor-model](https://github.com/henryletourneux/quant-equity-factor-model). The original implementation is acknowledged as the starting point for further development and research.

## Disclaimer

This project is intended for educational and quantitative research purposes only. Backtested performance does not guarantee future investment returns. Nothing in this repository constitutes financial or investment advice.
