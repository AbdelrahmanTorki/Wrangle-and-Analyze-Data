# Wrangle-and-Analyze-Data

Wrangling Data about dogs and their ratings from  @dog_rates twitter page using tweepy API, then cleaning and briefly analyzing the data

## Files Description:

The data is collected from three different sources:

1. Tweets Data given by udacity. (twitter-archive-enhanced.csv)
2. Some additional features of the same tweets collected through tweepy API .e.g favority count, number of retweets (tweet_json.txt)
3. A machine algorithm pre-implemented on dogs pictures that identify whether the picutre is a dog or not and if so, 
which breed it belongs to. (image_predictions.tsv) provided by Udacity


Wrangling and cleaning the data is done in wrangle_act.ipynb notebook


## Data Description: 

* image_predictions.tsv

    * tweet_id:  is the last part of the tweet URL after "status/" → https://twitter.com/dog_rates/status/889531135344209921
    * p1: is the algorithm's #1 prediction for the image in the tweet → golden retriever
    * p1_conf: is how confident the algorithm is in its #1 prediction → 95%
    * p1_dog: is whether or not the #1 prediction is a breed of dog → TRUE
    * p2: is the algorithm's second most likely prediction → Labrador retriever
    * p2_conf: is how confident the algorithm is in its #2 prediction → 1%
    * p2_dog: is whether or not the #2 prediction is a breed of dog → TRUE
    etc.

* tweet_json.txt, twitter-archive-enhanced.csv
	To best understand those files, its advisable to revise the tweet object at twitter developer website [Tweet Object](https://developer.twitter.com/en/docs/tweets/data-dictionary/overview/tweet-object.html)
