# Ensemble & Deep Learning Benchmarks for Renewable Energy Forecasting

Independent implementation and benchmarking work on machine learning approaches for
renewable energy (wind/solar) generation and demand forecasting — ensemble tree models,
an LSTM, ARIMA baselines, and a probabilistic transformer pipeline, evaluated on
synthetic data and the public EMHIRES European wind dataset.

This repository contains the underlying code and experiments developed as part of my
contribution to a paper submitted to **ICCTVB 2025** (International Conference on
Convergence of Technologies for Viksit Bharat), hosted by Sanjay Ghodawat University,
Kolhapur. The manuscript is currently in press; this repo shares the implementation and
methodology independently while the formal publication is finalized.

## What's here

- **`notebooks/ensemble_models_benchmark.ipynb`** — Core benchmark: Random Forest,
  XGBoost, LightGBM, and NGBoost (probabilistic) against a PyTorch LSTM sequence model,
  with paired statistical significance testing (Wilcoxon) between models.
- **`notebooks/energy_bench_prototype.ipynb`** — End-to-end prototype: synthetic data
  generation → ARIMA / Random Forest / Gradient Boosting baselines → battery storage
  simulation → economic metrics (PES / PEC / grid-related measures).
- **`notebooks/spg_wind_benchmark.ipynb`** — Benchmark pipeline against the public
  [EMHIRES wind generation dataset](https://data.jrc.ec.europa.eu/dataset/848d67ba-799e-46d9-a361-ae7d36b5c60e)
  (European Commission JRC), including a probabilistic transformer, interval
  calibration, and evaluation metrics/figures.
- **`data/synthetic_energy.csv`** — Synthetic dataset used for controlled experiments
  and baseline validation.

## Methodology summary

- Models compared: Random Forest, XGBoost, LightGBM, NGBoost, Gradient Boosting, ARIMA,
  and an LSTM sequence model.
- Metrics: MAE, RMSE, sMAPE, plus paired significance testing across models.
- Real-world validation on the EMHIRES wind dataset in addition to synthetic
  experiments.
- A battery energy storage system (BESS) simulation to translate forecast accuracy
  into downstream operational/economic impact.

## Status

Paper submitted and reviewed (Accept with minor changes) at ICCTVB 2025; publication
pending. This repository reflects the independent implementation work and will be
updated with the formal citation once the paper is published.

## Author

Tanmay Shinde — [GitHub](https://github.com/Tanny28) ·
[LinkedIn](https://linkedin.com/in/tanmay-shinde-840a05340) ·
[Portfolio](https://tanmay-shinde-28.vercel.app)

## License

Code in this repository is shared for portfolio/reference purposes. Please reach out
before reusing substantial portions.
