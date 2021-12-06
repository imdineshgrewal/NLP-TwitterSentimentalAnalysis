## Twitter Sentiment Analysis
The objective of this task is to detect hate speech in tweets. For the sake of simplicity, we say a tweet contains hate speech if it has a racist or sexist sentiment associated with it. So, the task is to classify racist or sexist tweets from other tweets.

Formally, given a training sample of tweets and labels, where label '1' denotes the tweet is racist/sexist and label '0' denotes the tweet is not racist/sexist, your objective is to predict the labels on the test dataset.
 
 
1. Understanding the Problem Statment
2. Tweets Preprocessing and Cleaning
   * Data Inspection
   * Data Cleaning
3. Story Generation and Visualization from Tweets
4. Extracting Feature from Cleaned Tweets
   * Bag-of-Words
   * TF-IDF
   * Word Embeddings
5. Model Building: Sentiment Analysis
   * Logistic Regression
   * Support Vector Machine
   * RandomForest
   * XGBoost
6. Model Fine-tuning
7. Summary

To classify a set of tweets into two categories:
   * racist/sexist
   * non-racist/sexist
  
## Data Files
 

**train.csv** - For training the models, we provide a labelled dataset of 31,962 tweets. The dataset is provided in the form of a csv file with each line storing a tweet id, its label and the tweet.><br/>
There is 1 test file (public)
<br/><br/>
**test_tweets.csv** - The test data file contains only tweet ids and the tweet text with each tweet in a new line.<br/><br/>


## Evaluation Metric:

The metric used for evaluating the performance of classification model would be F1-Score.<br/>

The metric can be understood as -
<br/>
**True Positives (TP)** - These are the correctly predicted positive values which means that the value of actual class is yes and the value of predicted class is also yes.<br/>

**True Negatives (TN)** - These are the correctly predicted negative values which means that the value of actual class is no and value of predicted class is also no.<br/>

**False Positives (FP)** – When actual class is no and predicted class is yes.<br/>

**False Negatives (FN)** – When actual class is yes but predicted class in no.<br/>

**Precision** = TP/TP+FP
<br/>
**Recall** = TP/TP+FN
<br/><br/>
 

**F1 Score** = 2*(Recall * Precision) / (Recall + Precision)
<br/><br/>
 

F1 is usually more useful than accuracy, especially if for an uneven class distribution.
