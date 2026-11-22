# Time Series Forecasting

This project explores daily sales forecasting with Python and
[StatsForecast](https://nixtlaverse.nixtla.io/statsforecast/). The
`timeseriesForecasting.ipynb` notebook compares baseline, ARIMA, seasonal
ARIMA, and cross-validation forecasts for bakery product sales.

## Getting started

### Run in Google Colab

Open the notebook directly in Colab:

[Open `timeseriesForecasting.ipynb` in Google Colab](https://colab.research.google.com/github/Atabak-Touri/forecasting-model/blob/main/timeseriesForecasting.ipynb)

The notebook installs its Python dependencies in the first cell.

### Run locally

Create an environment and install the dependencies:

```bash
python -m venv .venv
source .venv/bin/activate
pip install numpy pandas matplotlib statsforecast utilsforecast
```

Then launch Jupyter and open `timeseriesForecasting.ipynb`:

```bash
jupyter notebook
```

## Data format

The notebook expects a CSV file at
`sample_data/daily_sales_french_bakery.csv` with at least these columns:

| Column | Description |
| --- | --- |
| `unique_id` | Identifier for each product time series |
| `ds` | Observation date |
| `y` | Observed sales value |

Series with fewer than 28 observations are filtered out. The examples use
daily data and forecast the next seven days.

## What the notebook covers

- Plotting product sales series.
- Benchmarking `Naive`, `HistoricAverage`, `WindowAverage`, and
  `SeasonalNaive` models.
- Comparing non-seasonal ARIMA with seasonal ARIMA.
- Evaluating forecasts with mean absolute error (MAE).
- Using rolling-window cross-validation to compare model performance.

The notebook's examples use the `BAGUETTE` and `CROISSANT` series.
