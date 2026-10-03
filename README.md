# Nifty 50 Next-Session Forecast

Research code for forecasting the next trading session of the Nifty 50: data download, feature/volatility models (GARCH, GBM, LSTM), directional engines, intraday strategies and backtests.

## Contents

| File | What it is |
|------|------------|
| `archive/quant_all.py` | Quant Direction Engine v2 |
| `archive/quant_all_v2.py` | Quant Direction Engine v2 |
| `archive/quant_all_v3.py` | Quant Direction Engine v2 |
| `notebooks/Copy_of_LSTM_Time_Series_Forecasting.ipynb` | Copy of LSTM Time Series Forecasting |
| `notebooks/Price_Prediction_using_LSTM_and_TA.ipynb` | Price Prediction using LSTM and TA |
| `src/daata.py` | daata |
| `src/data_download.py` | data download |
| `src/direction.py` | direction |
| `src/download_all_data.py` | download_all_data.py |
| `src/download_all_entities_data.py` | download_all_data.py |
| `src/entities_universe.py` | entities_universe.py |
| `src/fetch_price.py` | fetch price |
| `src/garch_module.py` | garch module |
| `src/gbm_factory.py` | GBM model factory. |
| `src/intraday_orb_strategy_5min.py` | Nifty Intraday ORB-Retest Strategy (prediction-filtered) |
| `src/intraday_vol_regime_brain.py` | intraday vol regime brain |
| `src/nifty_forecast.py` | nifty_forecast.py |
| `src/nifty_forecast_all.py` | nifty_forecast.py |
| `src/nifty_forecast_minus.py` | nifty_forecast.py |
| `src/nifty_pipeline_v2.py` | Nifty Next-Day OHLC Forecast Pipeline -- v2 |
| `src/nifty_predict_report.py` | nifty predict report |
| `src/nifty_xabcd_backtest.py` | Nifty 30-min ORB 15-min-close breakout  ->  sell 0.4-delta option |
| `src/niftyprediction.py` | niftyprediction |
| `src/numpy_lstm.py` | numpy lstm |
| `src/plot_tradingview_chart.py` | plot tradingview chart |
| `src/pred1.py` | pred1 |
| `src/quant_all_v4.py` | Quant Direction Engine v2 |
| `src/quant_direction_engine.py` | quant direction engine |
| `src/quant_high_v2.py` | *** HIGH VARIANT *** |
| `src/quant_low_v2.py` | *** LOW VARIANT *** |
| `src/volume2.py` | ================================================================================ |

## Getting started

```bash
git clone https://github.com/<your-username>/nifty50-next-session-forecast.git
cd nifty50-next-session-forecast
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
pip install jupyterlab
jupyter lab   # then open a notebook in notebooks/
```

## Notes

- This is research code, not investment advice. Backtests do not guarantee future results.
- Market data is downloaded by the scripts in `src/` (see `download_*.py`, `fetch_price.py`); no data is committed to the repo.
