.. -*- mode: rst -*-
.. _forecasting:

.. currentmodule:: feature_engine.timeseries.forecasting

Model Monitoring
====================


Machine learning is becoming increasingly popular for time series forecasting because of its ability
to model complex relationships and handle large datasets. While traditional forecasting methods like
moving averages, ARIMA (autoregressive integrated moving averages), exponential smoothing, and others,
are effective in identifying trend and seasonality, machine learning algorithms like linear regression,
random forests, or gradient boosted machines, can model complex patterns and incorporate exogenous
features, thereby resulting in accurate predictions.

However, to use machine learning to forecast time series data, we need to extract relevant features
and convert the data into a tabular format, so that it can be framed as a regression problem.

Feature-engine's time series forecasting transformers give us the ability to extract and generate
useful features from time series to use for forecasting. They are built on top of Python libraries
such as Pandas and offer an interface to extract various features from temporal data simultaneously.

Time series forecasting involves learning from historical data observations to predict future values.
Feature-engine's offers various transformers for creating features from the past values.


Lag and Window Features
-----------------------

Trend and seasonality can be captured using lag and window features. In Feature-engine, we have
three transformers to extract these features.

Lag features
~~~~~~~~~~~~~

A lag feature at a given time step represents the value of the time series from a prior time step.
Feature engine's :class:`LagFeatures` implements lag features. These are straightforward to
compute and widely used in time series forecasting tasks. For instance, in sales forecasting,
you might include the sales from the previous day, week,
or even year to predict the sales for a given day. Lag features are also the foundation
to many autoregressive models like moving averages and ARIMA.

While lag features are particularly effective for capturing seasonality, they can also model
short-term trends. Seasonality is well captured by lag features because they carry data at
regular intervals from the past - like daily, weekly, or yearly cycles. For example, a 7-day
lag can capture weekly seasonality, such as sales spikes over the weekend; and a 365-day lag
can capture yearly seasonality, like Christmas holiday sales. Hence a machine learning model
can understand a lot of the time series patterns by using lag features as input.

However, lag features may not capture long-term trends unless they are combined with other features,
such as rolling window or expanding window features.

Window features
~~~~~~~~~~~~~~~


Expanding Window Features
~~~~~~~~~~~~~~~~~~~~~~~~~~


Forecasting Features Transformers
---------------------------------

.. toctree::
   :maxdepth: 1

   core_concepts
   setting_up
   visualization
  

|
|
|
