# Electricity Load Forecasting: LSTM vs. Classical Models

This repository contains a comparative analysis of time-series forecasting models applied to the American Electric Power (AEP) dataset. The project demonstrates the implementation and evaluation of both classical statistical methods and deep learning architectures for hourly energy demand prediction.

## Objective
To evaluate and compare the predictive performance of:
- **Classical Statistical Models:** Linear Regression (Normal Equation)
- **Deep Learning Models:** Long Short-Term Memory (LSTM) networks

## Dataset
- **Source:** American Electric Power (AEP)
- **Frequency:** Hourly
- **Task:** Univariate time-series forecasting

## Methodology
### Data Preprocessing
- MinMax normalization for feature scaling.
- Sliding window technique (24-hour look-back) for sequence modeling.
- Time-aware train-test splitting.

### Models Implemented
- **Linear Regression:** Served as the statistical baseline using the closed-form Normal Equation.
- **LSTM (PyTorch):** Recurrent neural network architecture optimized for capturing long-term temporal dependencies.

## Performance Comparison
- Linear Regression: MAE: 716.43 MW | RMSE: 956.31 MW
- LSTM Neural Network: MAE: 698.43 MW | RMSE: 931.18 MW

## Key Insights
- The LSTM model captures non-linear temporal dynamics more effectively than the linear baseline.
- Statistical models remain competitive for short-term forecasting tasks.
- Performance outcomes highlight the critical role of data preprocessing in time-series sequence modeling.

## Tech Stack
- Python
- PyTorch
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

## Future Work
- Incorporation of advanced statistical models such as ARIMA/SARIMA.
- Exploration of Transformer-based architectures for time-series forecasting.
- Expansion to multivariate forecasting (integrating external weather and socioeconomic variables).
- Rigorous hyperparameter optimization and cross-validation for deep learning models.

## Usage
1. Clone the repository.
2. Install dependencies: `pip install torch numpy pandas scikit-learn matplotlib`
3. Open and run the `AEP_Energy_Forecasting_LSTM.ipynb` notebook in a Jupyter environment.

---
*Developed as a professional study on Time Series Analysis and Deep Learning architectures.*
