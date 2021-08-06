# Scrapping Twitter Data Using Twint and Sentiment Analysis on the Scraped Data

This is a simple notebook to scrape the data from twitter using twint and analyze the data using nltk Sentiment Analyser and wordcloud.

**Objective**

 1) Whenever a company launches a new product, it is very imporatant to know the reaction and reviews of the customers. Twitter is one of the such platforms where people share their opinions about a product or anything.

2) This is a simple notebook to scrape and analyse the data from twitter using twint.

3) Although twitter does not represent the whole customer population (infact it may be less than 10% of the total customer population), but this analysis may give some important direction to the company that can define their future strategy. Besides it is very easy to get data from twitter as compared to other platforms (instagram, facebook). Also, twitter is fast in terms of getting reaction from the population. i.e. the moment product is launched, first reaction will be seen on twitter.

**Points to Note:**
1) There are two methods to scrape data from twitter. 1) Twitter API Collection via Tweepy 2) Non-API Collection via Twint

2) Tweepy uses official twitter api, but it limits the number of tweets that can be scrapped (depends on the pricing). It also requires your twitter developer account login etc. For free version, Our searches can only go back 7 days and we get 50 requests a month.

3) Twint is an OSINT (Open Source Intelligence) which uses twitter's own search feature, through which any public tweet can be accessed. There is no limit on the number of tweets that can be scraped using twint. There is no login required.

4) It looks like twint is better than tweepy but twint has consistency issues. And twint is very slow as compared to tweepy. Twint can only be used to scrape tweets, but tweepy can be used to interact with twitter, post tweets, automatic retweets, block user, DM a user etc. Read more about it using below links:

https://towardsai.net/p/nlp/methods-challenges-and-hazards-of-collecting-tweets-9e3e7805095a

https://towardsdatascience.com/what-python-package-is-best-for-getting-data-from-twitter-comparing-tweepy-and-twint-f481005eccc9

In this tutorial, we will use twint. Twint Library at github:
https://github.com/twintproject/twint

**Sentiment Analysis**
1) Here we will do sentiment analysis using nltk SentimentIntensityAnalyzer to identify postive, negative and neutral tweets.

2) Once positive and negative tweets are identified, we can create separate wordclouds for positive and negative tweets and identify which aspects/keywords/features customers liked and which customers did not like.
