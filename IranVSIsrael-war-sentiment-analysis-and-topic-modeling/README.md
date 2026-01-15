# Sentiment Analysis and Topic Modeling on Israel vs Iran War

## Overview

This project demonstrates social media analysis, which covers sentiment analysis and topic modelling towards Israel and Iran War.

## Step 1 - Preparation of the dataset
## Scraping comments from Youtube videos
In this stage, we have extracted Youtube comments from 14 Youtube videos from BBC, CNN, AL JAZEERA, SKY NEWS, ASSOCIATE PRESS, NBCNEWS, CGTN, FOX NEWS and 10 NEWS by python script using Youtube API and merged to one excel file. The scraper python script is included.

## Step 2 - Loading and Pre-processing

## Language Detection (Keep English Only)
Since Natural Language Processing in English language is mostly exploared and most comments are made by using English language, extracting English comments is important for simpicity.

### Lowercase
This is important to make same words treated as the same words.

### Remove URLs
URL's usuaally dont carry useful meaning for most NLP tasks like sentiment analysis and topic modeling.

### Remove Emojis
It is optional to remove or preserve emojis. In sentiment analysis it can be useful, but for this project simplicity it's removed. 

### Remove Punctuation
Punctuations don't usually help models understand meaning, so they're removed.

### Remove Numbers 
Numbers often add noise unless we're doing price prediction and dates analysis.

### Remove Stopwords 
This words appear very often but add little meaning.

### Lemmatization 
Lemmatization reduces words to their base or dictionary form(lemma). It is important to make different forms of the same word to be treated as the same. This technique is necessry for sentiment and classification.

## Step 3 - SENTIMENT GENERATION 
Used Pretrained Model named VADER which is great for Social Media Text, and clsifies comments as neutral, positive and negative.

## Topic Modeling 
This is important to find and identify the main topics/themes in the comments.


## Course

Social Network Analysis

