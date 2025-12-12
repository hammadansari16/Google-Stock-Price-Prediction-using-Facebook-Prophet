# Google-Stock-Price-Prediction-using-Facebook-Prophet

This project focuses on analyzing historical stock data for Google (GOOG) and forecasting future closing prices using Facebook Prophet, a robust library for time-series forecasting.

📋 Project Overview
The goal of this repository is to demonstrate how to visualize stock market trends and generate predictive models for financial data. By utilizing historical data dating back to 2004, the model attempts to predict the stock price behavior for the next 365 days.

🛠️ Technologies Used
Python: Core programming language.

Pandas: For data manipulation and cleanup.

NumPy: For numerical computations.

Matplotlib: For data visualization and plotting trends.

Prophet: An open-source forecasting procedure released by Facebook (Meta) for time series data.

📂 Dataset
The project utilizes a CSV file (GOOG.csv) containing historical stock information.

Data Shape: The dataset consists of approximately 4,120 records.

Key Features: Date, Open, High, Low, Close, Volume, Adj Close.

Timeframe: Starts from August 2004 (Google's IPO period).

🚀 Methodology
Data Loading & Inspection: The data is loaded using Pandas, and the shape and head are inspected to ensure data integrity.

Exploratory Data Analysis (EDA):

Visualized the historical "Closing Price" to understand the general upward trend and volatility over the years.

Data Preprocessing:

Prophet requires specific column names. The Date column was renamed to ds and the Close price column was renamed to y.

Model Training:

Initialized the Prophet model with daily_seasonality=True.

Fitted the model on the cleaned dataframe.

Forecasting:

Created a future dataframe extending 365 days into the future.

Generated predictions for these future dates.

Component Analysis:

Decomposed the time series to analyze specific trends, including weekly, yearly, and daily seasonality.

📊 Results and Visualizations
The notebook generates several key insights:

Historical Closing Price: A plot showing the growth of Google stock from 2004 to present.

Forecast Plot: A chart displaying the predicted stock prices (the blue line) with a confidence interval (the shaded blue area), overlaid on the actual historical data (black dots).

Seasonality Components: Breakdowns showing:

The overall growth trend.

Weekly trends (e.g., stock performance on specific days of the week).

Yearly seasonality (e.g., performance in specific months).
