Stock Price Prediction Using Gradient Boosting 📊
Welcome to the Stock Price Prediction project! This repository contains the code, data, and insights for predicting stock closing prices using machine learning techniques. The goal is to utilize historical stock data to create an accurate prediction model that provides actionable insights.

Overview
This project focuses on:

Analyzing historical stock data from Exxon Mobil.
Using Gradient Boosting Regressor to predict the closing price of stocks.
Evaluating the model using metrics like RMSE (Root Mean Squared Error) and R² (R-squared) for accurate performance measurement.
Dataset
The dataset includes historical stock data with the following features:

Date: The trading date.
Open: Opening stock price.
High: Highest price of the day.
Low: Lowest price of the day.
Close: Closing stock price (target variable).
Adj Close: Adjusted closing price.
Volume: Number of shares traded.
Example snippet from the dataset:

Date	Open	High	Low	Close	Adj Close	Volume
Oct 19 2022	10125.0	10399.0	10123.0	10379.0	9628.0	20921700.0
The cleaned dataset is included in the file Exxon_Mobil_Cleaned.xlsx.

Methodology
Data Preprocessing:

Cleaned raw data for missing or inconsistent values.
Normalized features using Min-Max Scaling and Standard Scaling.
Model Training:

Applied Gradient Boosting Regressor with optimized hyperparameters:
n_estimators: 200
learning_rate: 0.05
max_depth: 6
Model Evaluation:

Cross-Validation: Average RMSE of ~424 on validation sets.
Test Set Results: RMSE of ~560 and R² of 96%.
Results
The model demonstrates high accuracy in predicting closing stock prices. Sample results for test data:

Sample	Actual Closing Price	Predicted Closing Price
1	3472.0	4363.12
2	6331.0	6649.04
3	10379.0	10160.07
Key Metrics:

R-squared (R²): 0.96 (96% variance explained by the model).
RMSE: ~560 on test data.
How to Use
Clone the repository:

bash
Αντιγραφή κώδικα
git clone https://github.com/YourUsername/Stock-Prediction-Project.git
cd Stock-Prediction-Project
Install dependencies:

bash
Αντιγραφή κώδικα
pip install -r requirements.txt
Run the Python script:

bash
Αντιγραφή κώδικα
python stock_prediction.py
View predictions and evaluation metrics.

Technologies Used
Programming Language: Python
Libraries:
pandas, numpy for data manipulation.
scikit-learn for machine learning and scaling.
matplotlib for visualizations.
Tools: Google Colab for development.
Business Applications
Predict future stock prices to guide investment strategies.
Analyze market trends using historical data.
Create scalable models for forecasting other assets.
Future Enhancements
Incorporate external economic indicators for improved accuracy.
Add live data integration for real-time predictions.
Test with other machine learning algorithms like XGBoost or LSTM.
Contributions
Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request with your improvements or ideas. Feedback is also appreciated through the Issues tab.

License
This project is open-source and licensed under the MIT License.
