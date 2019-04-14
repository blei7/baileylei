---
layout: post
title: Model evaluation
subtitle: regression metrics
category: blog
tags: Metrics, General
---

#### 1. Root Mean Square Error (RMSE)

One of the most common performance measures for regression models is the [Root Mean Square Error](https://en.wikipedia.org/wiki/Root-mean-square_deviation) (RMSE).

![](/img/2019-04-14/RMSE.png)

Figure 1. shows a simplified version of the RMSE equation that measures the difference between what values or outputs the model predicts and what we actually observed in the data set.  In this metric, a lower RMSE score equates to a better fit.

Since the RMSE takes the square of the error prior to averaging, the equation will give more weight to larger errors, making it more sensitive to outliers. This can be good or bad depending on how we perceive the problem. For example, if large errors are undesirable, then RMSE will be more helpful.

#### 2. Mean Absolute Error (MAE)

[Mean Absolute Error](https://en.wikipedia.org/wiki/Mean_absolute_error) is another metric for regression.  The main difference between MAE and RMSE is that MAE averages the absolute differences (error) between observed and predicted values. In general, we can see that RMSE will produce a value greater than MAE. If the average magnitude of the error is the same, then RMSE will be the same as MAE. Whereas RMSE struggles with outliers, MAE is less prone to the effect of outliers.
