# Smart Meter Time Series Forecasting and Anomaly Detection

This repository contains an end-to-end pipeline for processing, modeling, and forecasting smart meter Advanced Metering Infrastructure (AMI) data. The project leverages XGBoost for time series forecasting of energy and demand, and incorporates a rule-based anomaly detection system for voltage faults.

## Project Structure

- **`Smart_Meter_Forcasting_Pipeline.ipynb`**: The main Jupyter Notebook detailing the entire pipeline:
  - Data loading and status filtering
  - Reindexing and missing value imputation (15-minute intervals)
  - Feature engineering and matrix definition
  - Model training (XGBoost) and chronological evaluation
  - Rule-based voltage anomaly detection
  - Rolling forecasts for production deployment
- **`demo.ipynb`**: A quick demonstration notebook for inference.
- **`models/`**: Directory for storing trained models (e.g., `.pkl` files).
- **`data/`**: Directory for datasets, including predictions and voltage bands.
- **`*.png`**: Feature importance visualizations for the trained models.

## Technologies Used
- Python
- Jupyter Notebook
- Pandas & Numpy for data manipulation
- XGBoost for time-series forecasting

## Getting Started

1. Clone this repository.
2. Ensure you have the required dependencies installed (`pandas`, `numpy`, `xgboost`, `scikit-learn`, `jupyter`, etc.).
3. Place your smart meter data inside the repository (make sure it's in the correct format).
4. Run the cells in `Smart_Meter_Forcasting_Pipeline.ipynb` sequentially to train the models and generate forecasts.

## Note
Trained models (`.pkl`) and generated datasets (`.csv`) are ignored in Git to prevent large binary files from clogging the repository history.
