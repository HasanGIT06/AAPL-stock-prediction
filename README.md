# 📈 AAPL Stock Prediction

This project uses **Long Short-Term Memory (LSTM)** networks to forecast AAPL stock closing prices based on historical data from December 12, 1980 to April 1, 2020.
The project covers Exploratory Data Analysis (EDA), data preprocessing, model training, and evaluation to compare the performance of baseline and modified LSTM architectures.

## ⚙️ Workflow

### 1. Exploratory Data Analysis (EDA)
- Analyzed historical AAPL closing prices to understand stock price trends and patterns.
- Visualized the stock price history to explore its movement over time.

### 2. Data Preprocessing
- Selected historical closing prices as the prediction target.
- Split the dataset chronologically into training and testing sets.
- Applied MinMaxScaler to normalize the data.
- Created time-series sequences using a 5-day lookback window.

### 3. Model Training
- Developed a baseline LSTM model with 50 LSTM units.
- Built a modified LSTM architecture with 63 LSTM units, Dropout, and a Dense layer.
- Used Early Stopping to monitor validation loss during training.

### 4. Evaluation
- Evaluated model predictions on the test set.
- Compared model performance using Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and Mean Absolute Percentage Error (MAPE).

## 📊 Results and Conclusion

| Model | RMSE | MAE | MAPE |
|---|---:|---:|---:|
| Baseline LSTM | 6.1176 | 4.1074 | 1.71% |
| Modified LSTM | 12.9486 | 8.4706 | 3.26% |

The **baseline LSTM achieved lower prediction errors** than the modified architecture across all three evaluation metrics.
This experiment demonstrates the implementation and evaluation of LSTM-based time-series forecasting, while highlighting that increasing model complexity does not necessarily improve predictive performance.
