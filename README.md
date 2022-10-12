## U.S.--Airline-Sentiment_project

Sentiment Analyses and Prediction Project

## Overview

There are six different airline companies in this dataset and their customers still complaining about some problems with their services/flights. We are going to analyze and making machine learning project for how airline companies could improve theirselves with our findings.

This is about why customers give airline negative,neutral or positive reasons. This will help airlines for further improvement.


## Business Problem

In this project, main goal is the analyze and predict airline sentiment(positive,neutral or negative) of flights depend on customer review's text with machine learning model. This will help airline companies for future work. Depend on customer's review airline companies could take action about it and improve theirselves.

## Dataset

The dataset provided on https://www.kaggle.com/crowdflower/twitter-airline-sentiment by ** Crowdflower's Data for Everyone library**.

Dataset has 14,640 entries and 15 columns.

We have 6 different major U.S. airline companies; United, Us Airways, American , Soutwest,
Delta and Virgin America.

All the tweets scraped at 2015 February.

We have three different target category as positive, neutral or negative depend on tweet.


## Exploratory Data Analysis(EDA)

negative     0.626913
neutral      0.211680
positive     0.161407

## Tweet Counts per Airline Companies
<img width="840" alt="Screen Shot 2022-10-12 at 10 43 11 AM" src="https://user-images.githubusercontent.com/5207341/195299031-d24d30b4-e9d0-4888-aef4-84d43a37cae6.png">


This graph basically shows us tweet counts per airline companies depend on our data.


## Sentiments per Airline Companies

![sentiment_per_airline_companies](https://user-images.githubusercontent.com/5207341/195295214-06e51f3d-c476-4e58-a53c-e0767965ccde.png)

Green bars shows us negative tweets and obviously negatives are really higher than others.


## Negative Reasons


![negative_reasons](https://user-images.githubusercontent.com/5207341/195295330-6d44a1d5-e62b-4ae9-9657-94bbe4e89a2f.png)

Customer Service Issue and Late Flight leads for general negative reasons from customer reviews.

## Negative Reasons per Airline Companies


![Negative Reasons per Airline Companies](https://user-images.githubusercontent.com/5207341/195295493-e9bfbaec-52a5-4e16-91ec-fc8c2643b47d.png)

First of all Customer Service Issue leads for most of airline companies for negative reason as expected from previous graph. United airlines second problem `Late Flight` apperantly big problem for this airline for count compare to other airlines. And also lost luggage problem is higher at the United airlines than others.

At Delta airlines instead of customer service late flight leads for negative reason.

And for Virgin America booking problems look like a needs to be work on.





## Modeling


The main metric that I would be using to assess my models performance is accuracy score. Because each class equally important for us. We want to predict every class equally. Not focusing only positive or negatives. Every class important for this project.


## CountVectorizer

1. Logistic Regression Score : 0.74
2. Naive Bayes Score         : 0.77
3. Ada Boost Score           : 0.75


## TF-IDF

1. Naive Bayes Score         : 0.70
2. Logistic Regression Score : 0.77
3. Random Forest Score       : 0.68
4. Gradient Boosting Score   : 0.73


This scores calculated on `test sets`. 

## Sequential

1. First Model Score      : 0.7845
2. Second(Improved) Model : 0.9286


Last Model visuals;

![sequential](https://user-images.githubusercontent.com/5207341/195297627-67f8a2a8-c881-4851-bc7d-6ef834a1fa88.png)

![confusion matrix](https://user-images.githubusercontent.com/5207341/195297700-3032ff2c-48e1-4e71-bb14-8c2f6202b971.png)

## Future Step

We can work on detail text and improve our model.
For example we still get little bit of false positive,neutral or negatives. We would work why is that and what we could do more on our model.
Also gather more tweets about these airline companies



