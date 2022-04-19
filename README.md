# **Machine Learning in PySpark**

## I. Repository Overview

- This repository contains multiple tutorials that cover building machine learning models in `PySpark` framework. In python notebook files `Spark` session was created, whereas in `Databricks` notebooks no such session was created, rather all computations were done using clusters on Databricks community edition.
- Currently 3 tutorial notebooks are available in this repository:
  1. `pyspark_regression.ipynb`
  2. `pyspark_classification.ipynb`
  3. `databricks_regression.html`
  
## II. Tutorial notebooks details

1. **`pyspark_regression.ipynb`**
    - This notebook covers developing a machine learning model in `PySpark` environment.
    - Dataset used for analysis is [Sarah Gets a Diamond](http://store.darden.virginia.edu/sarah-gets-a-diamond) taken from University of Virginia, Darden Business Publishing. I have purposefully and randomly removed values from 30 rows for two different columns, so that different data transformation and imputation techniques using PySpark functionalities(`pyspark.sql`, `pyspark.ml` in this case) can be applied.
    - A regression model is developed on this dataset to calculate the price(Y variable) of a diamond based on its multiple physical attributes/features(X variables).
    - Different data transformations, data imputation techniques, data aggregation using PySpark functionalities are applied for cleaning, imputing, pre-processing, and extracting summary statistics on model development data.
    - Regression model developement and tuning is performed using PySpark functionalitiess(`pyspark.ml.regression`, `pyspark.ml.tuning`, `pyspark.ml.evaluation` in this case).

2. **`pyspark_classification.ipynb`**
     - This notebook covers developing a machine learning model in `PySpark` environment.
     - Dataset used for analysis is [SMS Spam Collection Data Set](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection) taken from UCI Machine Learning Repository. A binary classification model is developed on this dataset to identify if the given text message a `Spam` message or a `Ham` message.
     - Different data transformation and NLP techniques(`lemmetizing`, `tf-idf` etc in this case) using PySpark functionalities(`pyspark.sql`, `pyspark.ml` in this case) are applied together for Text cleaning and pre-processing.
     - Classification model developement and tuning is performed under PySpark functionalities(`pyspark.ml.classification`, `pyspark.ml.tuning`, `pyspark.ml.evaluation` in this case).

3. **`databricks_regression.html`**
     - This notebook covers developing a machine learning model in PySpark framework on Databricks.
     - Dataset used for analysis is [Sarah Gets a Diamond](http://store.darden.virginia.edu/sarah-gets-a-diamond) taken from University of Virginia, Darden Business Publishing. I have purposefully and randomly removed values from 30 rows for two different columns, so that different data transformation techniques in PySpark framework can be applied.
     - A regression model is developed on this dataset to calculate the price(Y variable) of a diamond based on its multiple physical attributes/features(X variables).
     - Different data transformations, data imputation techniques, data aggregation using PySpark functionalities(`pyspark.sql`, `pyspark.ml` in this case) are applied for cleaning, imputing, pre-processing, and extracting summary statistics on model development data.
     - Regression model developement and tuning is performed using PySpark functionalities(`pyspark.ml.regression`, `pyspark.ml.tuning`, `pyspark.ml.evaluation` in this case).
     - Two major additions in the workflow in `databricks_regression.html` that were absent in `pyspark_regression.ipynb` :
       -  Using Databricks' functionalities to write `SQL` queries using *magic commands* and plot graphs using inbuilt Databricks plotting functionalities 
       -  In this tutorial I have combined pre-processing and modelling steps into a single model pipeline.
