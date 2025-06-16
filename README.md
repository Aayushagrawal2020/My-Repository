# Stock Market Prediction and Trading Strategy

This project explores different machine learning models to predict the next-day trend of the NASDAQ index and demonstrates a simple trading strategy based on these predictions.

## Project Overview

The goal of this project is to build models that can predict whether the NASDAQ (^IXIC) closing price will increase or decrease on the following day. It uses historical stock data, performs feature engineering, trains various machine learning models, and evaluates their performance. A basic trading model is also implemented to visualize the potential outcome of using the predictions.

## Models Used

The project implements and compares the following models:

-   **Support Vector Machine (SVM):** A linear SVM is used for classification.
-   **Linear Regression:** Used to predict the actual return of the NASDAQ.
-   **Random Forest Classifier:** An ensemble learning method for improved classification accuracy.
-   **XGBoost Classifier:** A gradient boosting framework, with hyperparameter tuning using GridSearchCV for optimized performance.

## Features Engineered

The models are trained on features derived from historical stock data. These include:

-   Daily Open, High, Low, Close, and Volume (percentage change)
-   Lagging historical returns
-   Volatility (rolling standard deviation of returns)
-   Moving Averages (5, 10, and 20-day)
-   Relative Strength Index (RSI)

## Trading Strategy

A simplified trading strategy is implemented:

-   If the model predicts an upward trend, the model "buys" (holds a long position).
-   If the model predicts a downward trend (for the RandomForest and XGBoost models with refined predictions), the model "sells" (holds a short position in the updated version of the trading model).

The performance of this strategy is visualized by tracking the portfolio value over time.

## Project Structure

The provided code is in the form of a Google Colab notebook. The key steps are:

1.  **Fetching Stock Market Data:** Downloading historical data for NASDAQ, S&P 500, and DJIA using `yfinance`.
2.  **Feature Engineering:** Creating relevant features for the models.
3.  **Train-Test Split:** Splitting the data into training and testing sets.
4.  **Model Training:** Training the SVM, Linear Regression, Random Forest, and XGBoost models.
5.  **Model Evaluation:** Assessing the performance of the classification models using accuracy and a classification report, and the regression model using Mean Squared Error (MSE).
6.  **Feature Importance (XGBoost):** Visualizing the importance of the engineered features for the XGBoost model.
7.  **Trading Model:** Implementing and visualizing the simple trading strategy.
8.  **Model Comparison:** Creating a comparison table of the models and their performance/features.
9.  **Learning Curve:** (Demonstrative) Plotting a learning curve to illustrate potential overfitting/underfitting.

## How to Run

1.  Open the provided Google Colab notebook.
2.  Run all the cells sequentially.
3.  Ensure you have the necessary libraries installed (the notebook includes commands to install/upgrade them).

## Libraries Used

-   `numpy`
-   `pandas`
-   `yfinance`
-   `scikit-learn`
-   `xgboost`
-   `matplotlib`

## Future Enhancements

-   Include more advanced technical indicators.
-   Explore different time periods and markets.
-   Implement more sophisticated trading strategies with risk management.
-   Consider time series cross-validation for more robust model evaluation.
-   Build a more comprehensive backtesting framework.
-   Explore deep learning models.

## License

This project is licensed under the MITWPU License.
