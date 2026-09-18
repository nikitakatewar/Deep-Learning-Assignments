# Deep Learning Assignment 4

## Problem Statement

Develop an LSTM-based model for time-series forecasting using stock price, weather, or sales datasets.

## Dataset

**Stock Price Dataset**

The **Close Price** is used for forecasting.

- Time step: 60 days
- Train-Test Split: 80:20

## Tools and Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- TensorFlow/Keras
- Scikit-learn

## Algorithm

1. Load the stock price dataset.
2. Select and visualize the Close price.
3. Normalize the data using Min-Max Scaling.
4. Create sequences using previous 60 days.
5. Split data into training and testing sets.
6. Create a two-layer LSTM model.
7. Compile using Adam optimizer and MSE loss.
8. Train the model for 20 epochs.
9. Predict stock prices.
10. Calculate MAE and RMSE.
11. Plot actual and predicted prices.

## Model Architecture

- LSTM Layer – 50 units
- LSTM Layer – 50 units
- Dense Output Layer – 1 neuron

## Results

| Metric | Value |

| MAE    | 3.0614 |
| RMSE   | 3.4350 |

The actual and predicted stock prices were visualized using a graph.

## Conclusion

The LSTM model was successfully implemented for stock price time-series forecasting. The model learned temporal patterns from historical stock prices and generated predictions for the test data.
