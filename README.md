# fake_news_detection using LIAR LIAR Dataset
USed NAive modelling with TFIDF and CBOW

Neural network( LSTM )
Multimodel keras layer

LIAR-PLUS is a benchmark dataset for fake news detection, released recently. This dataset has evidence sentences extracted automatically from the full-text verdict report written by journalists in Politifact. It consists of 12,836 short statements taken from POLITIFACT and labeled by humans for truthfulness, subject, context/venue, speaker, state, party, and prior history. For truthfulness, the LIAR dataset has six labels: pants-fire, false, mostly-false, half-true, mostly-true, and true. These six label sets are relatively balanced in size.

There are two tasks:

Binary classification task (true, false)
Six-way classification task (pants on fire, false, mostly false, half-true, mostly true, true) Your task is to select a classifier (or a group of classifiers) that you think is suitable for this dataset and get the highest possible accuracy. You can choose different classifiers for the two tasks. You are free to use any ideas you think will be suitable for this dataset. For example, you may plot graphs for gaining insights about the features or clean/re-organise the data for feature extraction.
