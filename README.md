### Predicting Stock Price From Historical Data

**Zaid Aboush**

#### Executive summary
This capstone project is about predicting stock market prices on which a decision can be made on whether to buy, hold or sell. 
#### Rationale
Why should anyone care about this question? Predicting stock price may help people focus their resources to obtain better return of investment and grow financially. 

#### Research Question
What are we trying to answer? How an accurate ML model can be build to predict future stock price(s)

#### Data Sources
What data will you use to answer you question? My instructor provided me with a historical Netflix stock prices that goes all the way back to 2018, here is the link: https://www.kaggle.com/datasets/jainilcoder/netflix-stock-price-prediction?select=NFLX.csv

#### Methodology
What methods are we using to answer the question? In this project I have been using various techniques to estimate future stock prices:
1-	Decision Tree: I used historical Open and Volume data as input features and closing price data as target variable after splitting the data (90% training & 10 testing).
2-	Support Vector Regressor (SVR): SVM is a classification algorithm used for predicting discrete categories, while SVR is a regression algorithm used for predicting continuous numerical values, hence SVR is more suitable for predicting stock price. Here, we will initialize and train a 'SVR' model using the scaled training features ('X_scaled_train') and target variable ('y_scaled_train').
3-	Time series analysis such as ARIMAX: ARIMAX (Autoregressive Integrated Moving Average with Exogenous variables) is a statistical model used for time series forecasting that extends the ARMA model by including external factors. It predicts a dependent variable using its own past values (Autoregressive), past forecast errors (Moving Average), and differencing to make the series stationary (Integrated). The "Exogenous" (X) component incorporates external variables that can influence the target variable, making it more accurate for complex systems like forecasting financial markets. 'X_scaled_train' and 'X_scaled_test' will be used as exogenous variables for ARIMA-X model, then define and train an ARIMA-X model using the same (p, d, q) orders as the ARIMA model and 'X_scaled_train'. Subsequently, make predictions on the test set using 'X_scaled_test', and finally, evaluate the ARIMA-X model's performance with MSE and R-squared, visualize predictions against actual values, and summarize findings.

#### Results
What did your research find?

#### Next steps
What suggestions do you have for next steps? Look into other company stock price prediction such as Qualcomm and try to incorporate other input features like technical indications that may includes RSI, MACD, or Bollinger Bands.

#### Outline of project

- https://github.com/zaboush/Module_20_Assignment_20p1/blob/main/Netflix_Stock.ipynb


##### Contact and Further Information
