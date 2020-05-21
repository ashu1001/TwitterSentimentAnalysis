# Twitter Sentiment Analysis

Sentiment Analysis is a term that you must have heard if you have been in the Tech field long enough. It is the process of predicting whether a piece of information (i.e. text, most commonly) indicates a positive, negative or neutral sentiment on the topic. In this article, we will go through making a Python program that analyzes the sentiment of tweets on a particular topic. The user will be able to input a keyword and get the sentiment on it based on the latest 100 tweets that contain the input keyword.

### Twitter API

This project requires you to have a Twitter Developer Account in order to prepare Training and test data. You can easily create your Twitter Developer account here: https://developer.twitter.com/en. After creating the account, you need to create an app and request consumer key and token key to get request from Twitter API. 

### Datasets

* **Training Data:** The training data will be prepared by calling the Twitter API for each of the Tweet ID mentioned in the Corpus dataset and getting the status for that. The link for Corpus data is [here](https://github.com/karanluthra/twitter-sentiment-training/blob/master/corpus.csv)(Note: The training set will take 10+ hours to prepare beacuse of Twitter API restriction, you can only request 180 times in a time period of 15 minutes. So, please be patient with that)

* **Test Data:** The test data will be prepared by calling the Twitter API for the particular search parameter and retreiving 100 latest tweets about that topic.

### Data Pre-processing

For data pre-processing steps of both of the datasets, we have followed the same methodology. Removing punctuation words, building the vocabulary and extracting word features for both the training and test set.

### Naive-Bayes Method

For this given project, we have use Naive-Bayes Classifier to classify given tweet as "postive","neutral" or "negative". The final model results will show whether sentiments for a particular tweet has been positive or negative depending on the majority.
