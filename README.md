# Human-activity-detection

Problem statement is taken from: https://www.kaggle.com/uciml/human-activity-recognition-with-smartphones

Here based on human engineered features from sensors data various machine learning techniques are experimented with Raw data + Deep learning model.



    To achieve the accuracy of model par with Expert engineered features, various Deep_learning models are tried with Hyperparameter tuning

    LSTM deeper architecture (Stacking) & wider Architecture (Neurons in layers) are fine tuned to find the best params

    Batch_size for LSTM is also tuned to find the best Accuracy

    Bi-directional LSTM stacked with LSTM cell tried

    2-D convolutional neural network is tuned with following params as hyper params (Kernel size, Maxpooling layer, Dropout rate, Neurons in Dense layer)

    As we see in the table, the best LSTM has accuarcy of 96.1% which is in par with classical model with 561 Domain Expert engineered features

    The best CNN Architecture have 96.8% accuracy which is in par with classical model with 561 Domain Expert engineered features.

    Our Deep learning model almost abstracted details needed to achieve the classical model with 561 Domain Expert engineered features.

    Best model in terms of accuarcy:

    Deep_cnn > Double stacked LSTM > Bidirectional LSTM + LSTM

    Model_4, Model_6, Model_7, Model_8 outperformed the classical machinelearning model with Expert engineered features in terms of accuracy as metric
