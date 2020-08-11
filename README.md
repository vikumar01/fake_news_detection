# fake_news_detection using LIAR LIAR Dataset
USed NAive modelling with TFIDF and CBOW
LOgestic regression worked best
Neural network( LSTM )
Multimodel keras layer

LIAR-PLUS is a benchmark dataset for fake news detection, released recently. This dataset has evidence sentences extracted automatically from the full-text verdict report written by journalists in Politifact. It consists of 12,836 short statements taken from POLITIFACT and labeled by humans for truthfulness, subject, context/venue, speaker, state, party, and prior history. For truthfulness, the LIAR dataset has six labels: pants-fire, false, mostly-false, half-true, mostly-true, and true. These six label sets are relatively balanced in size.

There are two tasks:
Binary classification task (true, false)
Six-way classification task (pants on fire, false, mostly false, half-true, mostly true, true) Your task is to select a classifier (or a group of classifiers) that you think is suitable for this dataset and get the highest possible accuracy. You can choose different classifiers for the two tasks. You are free to use any ideas you think will be suitable for this dataset. For example, you may plot graphs for gaining insights about the features or clean/re-organise the data for feature extraction.

Feature Engineering:

1. Credit score: this includes historical count of inaccurate statements by each speakers. Based on the speakers history, total number of pants-fire, false, mostly false, half-true, mostly-true, and true are recoded in dataset. For instance, Hillary Clintonhas a credit history vector h = (40; 29; 69; 76; 7), which corresponds to his counts of “pants on fire”, “false”, “barely true”, “half true”, “mostly true” for historical statements. As this vector includes count of correct statement, so value 1 is subtracted from that label. Now, credit score for each speaker is computed using the formula:

The reason for using this credit score is to sort of increase the relative difference between the output activations between the fake and the real cases (As the credit score will be high incase of a publisher who publishes fake news compared to the someone who does less.)

2. Probabilistic sentiment and polarity: We have computed the Probabilistic sentiment and polarity of statement + justification as additional feature which helped in predicting.
*more about text blob with its paper reference*
* Image of the total data*

3. Emotion lexicon: The NRC Emotion Lexicon is a list of English words and their associations with eight basic emotions (anger, fear, anticipation, trust, surprise, sadness, joy, and disgust) and two sentiments (negative and positive).
