# Human-activity-detection

Problem statement is taken from: https://www.kaggle.com/uciml/human-activity-recognition-with-smartphones

Here model is built on top of human engineered features from sensors data + classical machine learning techniques are experimented
 
Then deeplearning model is developed with Raw data (Gyroscope and accelerometer data from smartphone) + Deep learning model. Both the results are compared.


### Problem Statement

* Accelerometer and Gyroscope readings are taken from 30 volunteers while performing the following 6 Activities. Given this data we have to predict the Activity

### Use case:

* This can be used in Smart watch, phone or fit bands

### Bussiness Impact

* This can be used as product features

### Data Cleaning

* Preprocessing of the data

* Duplicate removel

* Exploratory data analysis


### Algorithm Applied

* To achieve the accuracy of model par with Expert engineered features, various Deep_learning models are tried with Hyperparameter tuning

* LSTM deeper architecture (Stacking) & wider Architecture (Neurons in layers) are fine tuned to find the best params

* Batch_size for LSTM is also tuned to find the best Accuracy

* Bi-directional LSTM stacked with LSTM cell tried

* 2-D convolutional neural network is tuned with following params as hyper params (Kernel size, Maxpooling layer, Dropout rate, Neurons in Dense layer)

* As we see in the table, the best LSTM has accuarcy of 96.1% which is in par with classical model with 561 Domain Expert engineered features

* The best CNN Architecture have 96.8% accuracy which is in par with classical model with 561 Domain Expert engineered features.

* Our Deep learning model almost abstracted details needed to achieve the classical model with 561 Domain Expert engineered features.

* Best model in terms of accuarcy:

* Deep_cnn > Double stacked LSTM > Bidirectional LSTM + LSTM


### Feature Engineering (done by experts, alreday avalibale)

* These sensor signals are preprocessed by applying noise filters and then sampled in fixed-width windows(sliding windows) of 2.56 seconds each with 50% overlap. ie., each window has 128 readings. 
