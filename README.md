

📊 Stock Analysis & Prediction Web App
This Flask-based web application allows users to view live stock data, interactive charts, and predict future stock prices using Machine Learning models like Linear Regression and Random Forest. It uses Yahoo Finance API for fetching real-time stock data.

🔧 Features
Live stock price fetch (using yfinance)
1-year historical data visualization
Interactive charts with Plotly (line, volume, candlestick, moving average, daily returns)
ML-based prediction using:
Linear Regression (sklearn.linear_model)
Random Forest Regressor (sklearn.ensemble)
Live price API endpoint
Clean and user-friendly interface

🧠 Machine Learning Models Used
Linear Regression
from sklearn.linear_model import LinearRegression
Random Forest Regressor
from sklearn.ensemble import RandomForestRegressor

📁 Project Structure
vbnet
Copy
Edit
├── app.py
├── templates/
│   ├── index.html
│   ├── stock_analysis.html
│   └── error.html
├── static/
│   └── (optional CSS/JS)
├── README.md
🚀 How to Run

1. 📦 Install Required Packages
bash
Copy
Edit
pip install flask pandas plotly yfinance scikit-learn
2. ▶️ Run the App
bash
Copy
Edit
python app.py
Open your browser and go to:
📍 http://127.0.0.1:5000

✅ Supported Stocks
Amazon (AMZN)
Apple (AAPL)
Google (GOOGL)
Meta (META)
Microsoft (MSFT)
Netflix (NFLX)
Nvidia (NVDA)

🔗 API Endpoint
GET /get_live_price/<stock_name>
Returns the live price of a given stock in JSON.

Example:
json
Copy
Edit
{
  "live_price": 189.75
}

🧪 Example Predictions
The app trains on past stock data and predicts future trends using two models. These predictions are plotted for visual comparison against actual prices.

📌 Notes
Data is pulled using yfinance, so internet is required.

Ensure the stock name entered matches one from the supported list.
