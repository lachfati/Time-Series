# **Energy Consumption Forecasting Using Machine Learning**

This project applies machine learning techniques to forecast energy consumption using the PJME hourly energy consumption dataset. The objective is to predict future energy consumption based on historical observations. The workflow incorporates feature engineering, time series cross-validation, and XGBoost regression to achieve accurate predictions.

## **Requirements**

This project requires Python 3.x and the following libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `xgboost`

Install the required libraries with the command:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

## **Dataset**

The dataset used is the **PJME Hourly Energy Consumption Dataset**, which contains hourly energy consumption data for the PJM Interconnection electricity market from **2002 to 2018**.

- **Source:** [PJM Interconnection Data Repository](https://pjm.com)
- **Key Features:**
  - Hourly energy consumption values (MW)
  - Time-based trends and seasonality

## **Project Highlights**

- **Data Preprocessing:**
  - Handled missing values and outliers.
  - Generated time-based features (e.g., hour, day, month, season).

- **Feature Engineering:**
  - Derived lagged variables and rolling averages to incorporate temporal dependencies.
  - Created additional features such as holiday indicators and weather data (if applicable).

- **Modeling:**
  - Implemented **XGBoost Regression** for prediction.
  - Used **time series cross-validation** to evaluate model performance.

- **Evaluation Metrics:**
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Error (MAE)

## **Usage Instructions**

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/energy-forecasting.git
   cd energy-forecasting
   ```

2. Install the dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost
   ```

3. Run the analysis script:

   ```bash
   python forecast.py
   ```

## **Results**

- Forecasted energy consumption with a **mean RMSE of X** (replace "X" with your result) across multiple test sets.
- Visualized predicted vs. actual energy consumption trends, highlighting model performance.

