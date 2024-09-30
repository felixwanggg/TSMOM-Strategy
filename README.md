Time Series Momentum Strategy
This project applies a time series momentum (TSMOM) strategy to historical financial data. The strategy involves defining several key technical indicators, performing exploratory data analysis (EDA), feature selection using stepwise regression, and then applying a soft voting classifier to predict market movement. The data spans from 2018 to 2024, and the goal is to backtest the strategy and assess its performance.

Project Structure
Technical Indicators:

The project starts by defining several commonly used technical indicators, including:
TSMOM (Time Series Momentum): A rolling sum of past returns to identify trends.
MACD (Moving Average Convergence Divergence): A momentum indicator that shows the relationship between two moving averages of an asset's price.
Other indicators include SMA (Simple Moving Average), EMA (Exponential Moving Average), RSI (Relative Strength Index), and Bollinger Bands.
Exploratory Data Analysis (EDA):

We perform EDA to understand the distribution of data and the relationships between features. This includes:
Plotting histograms of the indicators.
Correlation heatmaps to identify potential multicollinearity.
Time series plots to visualize the data over time.
Feature Selection:

After calculating the indicators, a stepwise regression method is used to eliminate features that do not contribute significantly to the model's predictive power. This process selects the best-performing features while controlling for overfitting.
Modeling with Soft Voting Classifier:

We apply a soft voting classifier that combines multiple models (Random Forest, SVM, and XGBoost) to predict market direction.
The classifier uses majority voting to improve the robustness and accuracy of predictions.
