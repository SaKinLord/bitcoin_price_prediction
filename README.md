Bitcoin Price Prediction Project
This project is designed to perform time series forecasting using Bitcoin price data obtained from Binance. It consists of three main components: data retrieval, data preprocessing, and model training/prediction. Below are the project details and usage instructions.

📋 Project Description
financial_time_series.py:
Retrieves Bitcoin price data (open, close, high, low, volume) from the Binance API.

data_preprocessing.ipynb:
Cleans the raw data, performs feature engineering, and prepares it for model training.

bitcoin_price_prediction.ipynb:
Uses the neuralprophet model (or a similar deep learning model) to predict Bitcoin prices.

🛠 Setup
Requirements
Python 3.8+
Required Libraries
bash
Kopyala
Düzenle
pip install pandas numpy matplotlib seaborn python-binance tensorflow scikit-learn jupyter
Binance API Key
Create an API key in your Binance account.
In the project directory, create a .env file and add your keys:
python
Kopyala
Düzenle
API_KEY = "your_api_key"
API_SECRET = "your_api_secret"
🚀 Usage
Data Retrieval
Run the financial_time_series.py script to fetch data from Binance:

bash
Kopyala
Düzenle
python financial_time_series.py
Output: raw_bitcoin_data.csv

Data Preprocessing
Open the data_preprocessing.ipynb file in Jupyter Notebook and run all cells:

Missing data cleaning
Feature addition (Moving Average, RSI, etc.)
Data normalization
Output: processed_bitcoin_data.csv

Model Training and Prediction
Run the bitcoin_price_prediction.ipynb file:

Split the data into training and test sets
Train the neuralprophet model
Visualize prediction results
Output: Prediction graphs and metrics (MAE, RMSE)
