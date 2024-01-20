This repo optimizes signals from a linear model for trading.

Unlike traditional features/target settings, here we transform the features to learn the relationship between target and features. We explore how features change over time and whether there are patterns or trends that can be captured by adjusting parameters from linear regression. By adjusting parameters (`mu`, `sigma`), we can identify deviations or anomalies in the behavior of the features with respect to the target variable.

Variables are transformed to maximize PnL over the Sharpe Ratio criterion.

The nature of this exercise is unsupervised learning.

The ouput of the optimization results in a signal, which can then be later multiplied to features to produce a prediction.

The exercise trains continuously in-sample and predicts & trades out-of-sample. Features are scaled in-sample.

Only long positions are considered.

References:

https://github.com/Cnernc/OptimalLinearSignal
