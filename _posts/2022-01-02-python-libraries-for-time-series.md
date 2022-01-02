---
title: Best python libraries for Time Series Analysis
date: 2022-01-02
published: true
categories: [data_science]
header:
  teaser: '/../assets/images/python_lib_ts/teaser.PNG'
---

Time Series analysis involves a lot of tasks such as forecasting, classification, anomaly detection, time-series feature extraction, and sequence matching... etc.

For each of these tasks, I have curated a list of the best time series python libraries.
![plotly time-series](/assets/images/python_lib_ts/teaser.PNG?raw=true){: .center-image }

**Prophet**

Facebook (Meta)’s `Prophet` is a generic time series forecasting at scale.

It follows the scikit-learn API, *fit* and *predict* methods so it should be easy to pick up for
anyone with experience with sklearn. At its core, the Prophet procedure is an additive regression model.

These are situations where Prophet is better than regular forecasting methods.

Mostly in demand forecasting business where:

- hourly, daily, or weekly observations with at least a few months (preferably a year) of history.
- important holidays that occur at irregular intervals that are known in advance.

> Key Takeaway : Good in modelling weekly, monthly, yearly and holiday seasonal components.

Working example of Prophet.

**tsai**

There is a cool library that provide easy to use state of the art Deep Learning models for time series analysis.

`tsai` is an open-source deep learning package built on top of Pytorch & Fastai

- Fine-tuned model architectures.
- Easy to change/swap any models without modifying much in the code base.
- Provide support for large dataset to fit in memory.
- Easy data preparation.
- Supports time-series classification, regression and forecasting...

Here's a list with some of the state-of-the-art models available in `tsai`:

1. [LSTM](https://github.com/timeseriesAI/tsai/blob/main/tsai/models/RNN.py) (Hochreiter, 1997) ([paper](https://ieeexplore.ieee.org/abstract/document/6795963/))
2. [mWDN](https://github.com/timeseriesAI/tsai/blob/main/tsai/models/mWDN.py) - Multilevel wavelet decomposition network (Wang, 2018) ([paper](https://dl.acm.org/doi/abs/10.1145/3219819.3220060))
3. [MLSTM-FCN](https://github.com/timeseriesAI/tsai/blob/main/tsai/models/RNN_FCN.py) - Multivariate LSTM-FCN (Karim, 2019) ([paper](https://www.sciencedirect.com/science/article/abs/pii/S0893608019301200))
4. [InceptionTime](https://github.com/timeseriesAI/tsai/blob/main/tsai/models/InceptionTime.py) (Fawaz, 2019) ([paper](https://arxiv.org/abs/1909.04939))
5. [TabTransformer](https://github.com/timeseriesAI/tsai/blob/main/tsai/models/TabTransformer.py) (Huang, 2020) ([paper](https://arxiv.org/pdf/2012.06678))

>Key Takeaway : The models provided by this library are very powerful and complex.
These models/architectures are still too new to be used in a real-world situation.

Working example of tsai.

**tsfresh**

It calculates a significant number of time series characteristics, or features, automatically. 

These features can then be used for regression or classification tasks in the future.

To develop a model, it first calculates a huge number of features and then narrows it down by selecting just relevant features. The feature extraction and the feature selection offer the possibility of parallelization.

>Key Takeaway : Shorten the time spent manually extracting and selecting features for every regression or classification problem. Especially while performing tasks for which one lacks domain expertise.

Working example of tsfresh.

**stumpy**

STUMPY is a powerful and scalable library that efficiently computes something called the [matrix profile](https://stumpy.readthedocs.io/en/latest/Tutorial_The_Matrix_Profile.html), which can be used for a variety of time series data mining tasks such as:

- pattern/motif (common subsequence in time-series) discovery
- anomaly detection
- shapelet discovery

At its core, the STUMPY library efficiently computes something called a matrix profile, a vector that stores the z-normalized Euclidean distance between any subsequence within a time series and its nearest neighbor.

>Key Takeaway : A Unique way to do anomaly detection and motif discovery by comparing the distance between subsequences within the time-series.

Working example of stumpy.

**statsmodels**

statsmodels is a Python package that provides a complement to scipy for statistical computations including descriptive statistics and estimation and inference for statistical models.

**`[statsmodels.tsa](https://www.statsmodels.org/stable/tsa.html#module-statsmodels.tsa)`** contains model classes and functions that are useful for time series analysis. 

Basic models include univariate autoregressive models (AR), vector autoregressive models (VAR) and univariate autoregressive moving average models (ARMA).

`statsmodels.tsa.stattools`  contains many useful functions for Descriptive Statistics and Tests such as acf, pacf, granger-causality, adf unit root test, kpss test, bds test, ljung-box test and others.

>Key Takeaway : Provide best tools to do any kind of statistical/Classical time-series analysis.

Working example of statsmodels.

**Boosting models**

Boosting models include XGBoost, LightGBM and CatBoost.

These are the most popular tree ensemble models, with many Kaggle competitions won using them. For tabular data, they even outperform Deep Learning models. We can also transform our time-series data into tabular data (link), and then can use these models.

>Key Takeaway : Nowadays these models are giving state of the art results with model interpretability in hand (easy integration with SHAP and LIME), fast to train and even provide GPU support.

Working example of Boosting model for time-series.

**Kats**

Recently Facebook (Meta)’s open-sourced another time series library which is a ***One stop shop for time series analysis in Python.***

It provide these functionalities:

- forecasting (10+ individual forecasting models, ensembling)
- anomaly/change point detections
- TSFeatures for time- series feature extraction

>Key Takeaway : This is the newest library on the list, but it offers some excellent forecasting and offline change point detection algorithms.

Working example of Kats.