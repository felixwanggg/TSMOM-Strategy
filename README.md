Time Series Momentum Strategy
=
This project applies a time series momentum (TSMOM) strategy to historical financial data. The strategy involves defining several key technical indicators, performing exploratory data analysis (EDA), feature selection using stepwise regression, and then applying a soft voting classifier to predict market movement. The data spans from 2018 to 2024, and the goal is to backtest the strategy and assess its performance.

Technical Indicators:
=
The project starts by defining several commonly used technical indicators, including:
TSMOM (Time Series Momentum): A rolling sum of past returns to identify trends.
MACD (Moving Average Convergence Divergence): A momentum indicator that shows the relationship between two moving averages of an asset's price.
Other indicators include SMA (Simple Moving Average), EMA (Exponential Moving Average), RSI (Relative Strength Index), and Bollinger Bands.


Exploratory Data Analysis (EDA):
=
I perform EDA to understand the distribution of data and the relationships between features. 

This includes:
Plotting histograms of the indicators.
Correlation heatmaps to identify potential multicollinearity.
Time series plots to visualize the data over time.

Feature Selection:
=
After calculating the indicators, a stepwise regression method is used to eliminate features that do not contribute significantly to the model's predictive power. This process selects the best-performing features while controlling for overfitting.

Modeling with Soft Voting Classifier:
=
I apply a soft voting classifier that combines multiple models (Random Forest, SVM, and XGBoost) to predict market direction.
The classifier uses majority voting to improve the robustness and accuracy of predictions.


Data
=
The dataset consists of historical financial data from 2018 to 2024. The data includes daily prices (open, close, high, low) and technical indicators derived from those prices.

Methodology
=
Technical Indicator Calculation:
=
Using the adjusted closing price of each asset, the project calculates various indicators that form the basis for the strategy.

Exploratory Data Analysis (EDA):
=
Before training the model, we perform EDA to check for patterns and relationships between features. 
This includes:
Visualizing the distribution of returns and technical indicators.
Checking correlations between features.

Stepwise Regression:
==
I eliminate irrelevant features using stepwise regression, ensuring that only the most relevant technical indicators are used for training the model.

Modeling:
==
I use a soft voting classifier composed of Random Forest, SVM, and XGBoost models to predict market direction.
The model is trained on data from 2018 to 2024, and the results are evaluated by comparing the cumulative return of the strategy versus the asset.

Results:
=
The strategy's performance is visualized by plotting the cumulative return of the strategy versus the asset over time. The model's performance is measured in terms of accuracy, Sharpe ratio, and cumulative returns.
