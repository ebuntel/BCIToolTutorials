# NAML Config File Parameter Guide

## General Parameters
The following parameters are required for every NAML config file:

* filePath: Relative path to the data file you wish to use.
loggingEnabled: If true will output logs as the program progresses.

* targetCol: The name of the column of your data you wish to classify by.

* percentTrain: The percentage of the initial dataset to be set aside for use as a testing set. This is only used if you choose the COLUMN_ENSEMBLE method.

## Jobs
Jobs: This is where you define what kind of classification you want to run. It is an array of jobs. Each job must be surrounded by braces ({}), and each job should be separated by a comma (,). Each job must contain the following:

* method: The method of classification you want to run. There are three options:

1. MULTIVARIATE_CLASSIFICATION: Allows you to classify using a multivariate classifier. 

2. UNIVARIATE_TRANSFORMATION: Allows you to classify using a univariate classifier by transforming the dataset into a univariate time series. 

3.  COLUMN_ENSEMBLE: Allows you to classify using univariate classifiers on specified columns of your data. 

* classifier: The classifier you want to use for this job. UNIVARIATE_TRANSFORMATION and COLUMN_ENSEMBLE have access to univariate classifiers only whereas MULTIVARIATE_CLASSIFICATION has access to multivariate classifiers only. Here are the names of the available classifiers:

- Univariate:
1. TSF_CLF: Time Series Forest

2. KNN_CLF: K Nearest Neighbors

3. PF_CLF: Proximity Forest

4. RISE_CLF: Random Interval Spectral Forest

5. EE_CLF: Elastic Ensemble

6. BOSSE_CLF: Bag of Symbols SFA Ensemblee

7. TDE_CLF: Temporal Dictionary Ensemble

8. W_CLF: Word ExtrAction for time SEries cLassification

- Multivariate:
1. MrSEQL: Mr-SEQL classifier

2. MUSE: Multivariate WEASEL+MUSE classifer
