# Short-Rate-Forecasting
A comparative study of short-term interest rate forecasting using stochastic models (Vasicek, CIR) and machine learning techniques (Random Forest, LSTM), applied to 13-week U.S. Treasury Bill rates with a rolling window framework and benchmarked against a Random Walk.

Models Implemented
🔹 Mathematical Finance

Vasicek Model
A mean-reverting interest rate model with constant volatility, estimated using Maximum Likelihood Estimation (MLE).
Cox-Ingersoll-Ross (CIR) Model
A non-negative, mean-reverting model with volatility proportional to the square root of the rate.

🔹 Machine Learning

Random Forest Regressor
An ensemble learning model based on decision trees that captures non-linear patterns in lagged rate data.
LSTM (Long Short-Term Memory)
A type of recurrent neural network (RNN) designed for sequence data, capable of learning time-dependent patterns

 Benchmark
Random Walk
Serves as the baseline model. Forecasts are generated assuming that the best estimate for tomorrow's rate is today's rate. All models are expected to outperform this naïve benchmark.

Methodology

All models are evaluated using a rolling window forecasting approach:
Window Size: 90 observations
Forecast Horizons:
1-step ahead (1 day)
7-step ahead (1 week)
30-step ahead (1 month)
90-step ahead (3 months)

Evaluation Metrics
Mean Squared Error (MSE): Measures the average squared difference between predicted and actual rates.
Directional Accuracy: Measures whether the model correctly predicts the direction of rate movement.
Visual Forecast Comparison: Plots model forecasts against actual rates for interpretability.



