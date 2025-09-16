# Revenue Forecasting Toolkit

Predictable, explainable revenue forecasts for subscription and transactional businesses.

## What’s inside
- `notebooks/` — exploratory analysis & model demos (Prophet, SARIMA, XGBoost)
- `src/` — reusable forecasting library (data pipeline, feature engineering, models)
- `examples/` — sample datasets and end-to-end scripts
- `reports/` — example PDF/HTML reports and dashboards
- `tests/` — unit tests & sanity checks
- `requirements.txt` — Python deps

## Features
- Baseline time-series (ETS/ARIMA/Prophet) and ML models (XGBoost)
- Automated backtesting and rolling-origin evaluation
- Uncertainty estimation: prediction intervals + scenario generation
- Feature importance & explainability (SHAP)
- Exportable forecast package: CSV, JSON, Power BI-ready data

## Quickstart
```bash
git clone git@github.com:rob-russell/revenue-forecasting-toolkit.git
cd revenue-forecasting-toolkit
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python src/run_pipeline.py --input examples/sample_revenue.csv --output forecasts/out.csv
