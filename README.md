# credict-card-detection
The project is carried out by collecting and cleaning data followed by creating model to
analyse data and finally visualizing it for better understand.
• The machine learning algorithm such as Neural Networks are used to obtain the results.

Data collection
• The datasets contains transactions made by credit cards in September 2013 by European
cardholders. This dataset presents transactions that occurred in two days, where we
have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the
positive class (frauds) account for 0.172% of all transactions.
• It contains only numerical input variables which are the result of a PCA transformation.
Unfortunately, due to confidentiality issues, we cannot provide the original features and
more background information about the data. Features V1, V2, … V28 are the principal
components obtained with PCA, the only features which have not been transformed
with PCA are ‘Time’ and ‘Amount’.
• Feature ‘Time’ contains the seconds elapsed between each transaction and the first
transaction in the dataset. The feature ‘Amount’ is the transaction Amount. Feature
‘Class’ is the response variable and it takes value 1 in case of fraud and 0 otherwise.


data pre-prepration
Since nearly all predictors have been anonymized, we decided to focus on the non-anonymized
predictors time and amount of the transaction during EDA. The data set contains 284,807
transactions. The mean value of all transactions is $88.35 while the largest transaction recorded
in this data set amounts to $25,691.16. However, as you might be guessing right now based on
the mean and maximum, the distribution of the monetary value of all transactions is heavily
right-skewed. The vast majority of transactions are relatively small and only a tiny fraction of
transactions comes even close to the maximum

Distribution of monetary value distribution
The time is recorded in the number of seconds since the first transaction in the data set.
Therefore, we can conclude that this data set includes all transactions recorded over the course
of two days. As opposed to the distribution of the monetary value of the transactions, it is
bimodal. This indicates that approximately 28 hours after the first transaction there was a
significant drop in the volume of transactions. While the time of the first transaction is not
provided, it would be reasonable to assume that the drop in volume occurred during the nigh

distribution of time feature
most transactions are non-fraudulent. In fact, 99.83% of the transactions in this data set were
not fraudulent while only 0.17% were fraudulent. The following visualization underlines this
significant contrast

prediction
Accuracy of naive bayes algorithm is 84.7%
Accuracy of logistic regression is 90.10%
Accuracy of neural network is 99.88%

Conclusion
Compared to the other machine learning algorithm the experiment shows Neural Networks have high Accuracy rate.

