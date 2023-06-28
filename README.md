# Project 2 -  Neural Network Recommender

### Project description
<p>The aim of this project was to create a neural network recommender based on real hotel data.</p>

## Data preprocessing

#### data_preparation file
<p>In this file I've done basic data preprocessing and filtering of raw data as well as aggregation of certain features into buckets. </p>

#### recommender_and_evaluation file

<p>As a base there is 6 <strong>categorical</strong> columns: <br>

    ['term', 'length_of_stay_bucket', 'rate_plan', 'room_segment', 'n_people_bucket', 'weekend_stay']

<p>For each user and item I extracted the most common label in every feature on which I later used one hot encoding getting 24 separate features. </p>

## Models

<p>I've tested NeuMF model and also mu custom model which I've named Enet</p> 

## Data preprocessing
<p>I've also prepared 2 types of data and tested models also on data without any preparation. I've come up with feature percentage and one hot encoding.</p> 

## Recommender testing and tuning

<p>I've did a few runs of combinations of my two chosen models and 3 ways of data preprocessing. The most promising model turned out to be the NeuMF as the hybrid model.</p>
<p>I've decided to play with it more and tune it. My final params are: </p>
{'batch_size': 96.0, 'embedding_dim': 88.0, 'lr': 0.0028545386506524557, 'n_epochs': 3, 'n_neg_per_pos': 2.0}

## Results
<p>My final results for hr10 metric is 0.244 which are better than both Amazon and Netflix recommender</p>

In this project I've everything clearly visible in the notebook so I hope it would be easier to understand than my previous one.



### Requirements to run
<pre>
- Python 3.9
- pip install -r requirements.txt
</pre>
