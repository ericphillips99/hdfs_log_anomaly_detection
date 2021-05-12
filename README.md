# hdfs_log_anomaly_detection
## Data 586 Advanced Machine Learning: Final Report
### Automated anomaly detection on HDFS (Hadoop Distributed File System) log files.
Log parsing and feature extraction was performed using the [LogParser](https://github.com/logpai/logparser) and [Loglizer](https://github.com/logpai/loglizer) libraries. Principle component analysis is used for dimensionality reduction, and models developed include logistic regression, KNN, Quadratic Discriminant Analysis, Random Forests, and Gradient Boosting Classification Trees, implemented in scikit-learn in Python. A tuned gradient boosting classifier is selected, and attains a weighted binary cross entropy loss of 0.0049 and an F1 score of 0.9978 on withheld 15% test set.