# IU_netsci
Project for Network Science course at IU

The Fitabase Graph Analysis notebook reads in fit3.csv dataset and produces 
- two graph datasets: 
    fit_graph_19.gexf (a coarse grain partitioning into 19 link communities) and 
    fit_graph_42.gexf (finer grain partition into 42 link communities)
- two spreadsheets describing each partitioned set of communities:
    fit_communities_19.csv
    fit_communities_42.csv
    
 M1 Data Collection notebook collected 10,000 tweets between 4/11/2018 and 4/17/2018 using the search terms #pizza and #yoga, using the Twitter API tweepy.  Unfortunately the tweets collection cannot be reproduced, as Twitter API does not expose tweets that are more than a week old.  To run this notebook please use your Twitter API user api_key and api_secret, as it has been removed from the public version of this notebook. This notebook produced two datasets of collected tweets: 
  #pizza-2018-04-17.csv 
  #yoga-2018-04-17.csv
 
 M2 Sentiment Analysis notebook reads tweet collection datasets and runs NLP algorithms from the Python nltk library to determine sentiment polarity for each tweet: positive, negative or neutral. It aggregates the counts of tweet favorites, followers, retweets and sentiments and produces visualizations comparing metrics for #pizza vs. #yoga tweets. It also calculates and compares the time it took to collect each type of tweets. 
