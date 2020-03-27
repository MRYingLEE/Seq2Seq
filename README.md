# DeepTime: deep learning framework for time series forecasting
This is a deep learning framework for time series forecasting. It uses Tensorflow+Karas as base.

# Why?

I have done a few time series forecasting projects. I hate I have to start from scratch every time, which always take hours to run your model.And I hate to tune the hyperparameters manually. I want to focus my problem only. And I want to start quickly.
I couldn't find a good framework to do so. So I decided to develop one for myself.

# Who?

This framework targets data scientists who wants to quickly start a time series forecasting model.

# What?

This is a deep learning framework for time series forecasting. It uses Tensorflow+Karas as base.
So, no pure statistics model was covered. Technically I use deep learning model, maybe along with some statistics model as part.
Time series (TS) data is focused. Technically 2 kinds of time-series data are supported.

Logically, time-series data has the 3D shape of (N_ series, n_timestamp, n_features).

Usually, time-series data can be categorized as:
## Tabular Data Source
Technically, Pandas (2D) with chunks (series, the 3rd D ).

Pros: Intuitive

Cons: Not efficient

## (Anonymous) 3D Array
Technically, NumPy array of (N_ series, n_timestamp, n_features).

Pros: Efficient and Neutral to NN

Cons: Not intuitive

These 2 kinds of data can be converted to each other easily.

## Different Usages for 2 kinds of TS data 

Some AutoML tools support tabular data source, some support 3d array with shuffle=False. 
Some neurual network scripts support tabular one, somes do 3d one.

## Some related questions:
Is this an autoML platform? NO!
Are there any built-in models? Yes, but only for reference.
Are there hyperparamerters tuning built in? Yes.

# Which?
Is this a whole pipeline framework? No, I won't cover data preprocessing, which can be covered by Time-series-Preprocessing-Studio-in-Jupyter (https://github.com/MRYingLEE/Time-series-Preprocessing-Studio-in-Jupyter ）.

# Technology
1. Tensorflow+Karas as deep learning framework. 
Tensorflow 2.x is preferred.
Don’t mix tensorflow.keras and keras.

2. NNI (https://github.com/microsoft/nni ) may be used as hyperparameters tuning tools.
3. Dataframe of Pandas instead of ndarray of Numpy will be used as basic data format. ndarray of Numpy will be used internally, but the data scientist need focus on Dataframe only.
4. Timeserio (https://github.com/octoenergy/timeserio ) may be used as a reference.
