# lstm-autoencoder-for-anomaly-detection
Using LSTM Autoencoder to Detect Anomalies and Classify Rare Events.

So many times, actually most of real-life data, we have unbalanced data. Data were the events in which we are interested the most are rare and not as frequent as the normal cases. As in fraud detection, for instance. Most of the data is normal cases, whether the data is already labeled or not, and we want to detect the anomalies or when the fraud happens.
When dealing with unlabeled data, we usually go to **"outliers detection"** methods such as [Isolation Forest](https://en.wikipedia.org/wiki/Isolation_forest), **Cluster-Based Local Outlier Factor (CBLOF)**, **Histogram-Based Outlier Detection (HBOS)** etc. While labeled data is considered as a **"classification"** problem and classifiers like [Support Vector Machine (SVM)](https://en.wikipedia.org/wiki/Support-vector_machine) and [Random Forest](https://en.wikipedia.org/wiki/Random_forest) are used. However, given the positive data points are rare in the data, the algorithm finds it difficult to learn so much from the data. A classifier for example, usually ends up predicting "negative" for all cases to achieve the best accuracy.
Here we will look at a different approach that can be used in both supervised and unsupervised [anomaly detection](https://en.wikipedia.org/wiki/Anomaly_detection) and rare event classification problems. **Long Short-Term Memory Autoencoders**. 
