# Natrual-Language-Processing
UCLA Master of Applied Economics Econ 423 Assignment

## Problem statement: 

How can we estimate the sentiment of Yelp reviews based on the text of the review? 

## How we will solve the problem: 

We will use star ratings of reviews from (1, 2, 3, 4, 5) to denote sentiment (Very Negative, Negative, Neutral, Positive, Very Positive). We will solve the problem using machine learning, using different types of machine learning models. We will mainly use the NLTK library. We will first convert the words in the text of the reviews into vectors. Then we will train various models, starting with a 70/30 split for train vs. validation, that will classify the review as one of the 5 categories we have above. We will initially judge the accuracy of the models using the validation set. 

## Topic and Description (from previous proposal): 

The topic of our project will be sentiment analysis and the primary data set we will use for the project will be the Yelp Open Dataset (https://www.yelp.com/dataset), which consists of over 4.7 million Yelp reviews and their corresponding ratings. We like this data set as it not only contains a huge body of text – which we can use for sentiment analysis – but also contains ground truth values for every review so that we can accurately judge how effectively and precisely our model can estimate sentiment from text. 

Since the data set is so large, we propose randomly sampling sets of 47,000 reviews (without repetition) from the data set, so that each sample is roughly 1% of our available data set, and has completely unique information. Then we can train our model using the 1st and 2nd samples, validate on the 3rd sample, and test using the 4th sample. Thus, we can potentially create a model using only 4% of our total data. Our model will judge sentiment by estimating the number of stars a review has based on the text in the review. 

#### The aforementioned model will be the primary goal of the project, and we hope to get the accuracy score of the model as high as possible through testing various types of features and models. We are particularly interested in finding out which models are best for predicting the sentiment of Yelp reviews. 

If time permits, we propose creating an ensemble of models using different 4%-sized chunks of the Yelp data set. Potentially, we could create an ensemble of 10 models, each using a different 4%-sized chunk of the data set, and still have only used 40% of the data available. Since the data set is so large, we could alternatively train our models on larger selections of data, for example on 94,000 reviews (around 2% of the data set) instead of on 47,000 reviews. 

Also, if we are able to develop a very accurate model for sentiment analysis relatively early in the quarter, and if we have the time, we propose testing our best model(s) based on the Yelp data on other types of review data, from product reviews on Amazon to movie reviews on IMDB, and possibly even on Tweets.  

We consider the above directions (and others) that we can take our project in as optional, and our primary goal for the project is to develop a very accurate model for estimating the sentiment of Yelp reviews, as well as to compare the effectiveness of different models for estimating the sentiment of Yelp reviews. 
 
