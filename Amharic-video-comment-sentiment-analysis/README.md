# Sentiment Analysis on Amharic music video

## Overview

This project demonstrates social media analysis on Ethiopian traditonal music called **ወንድ ልጅ ቆረጠ** sang by musician Dagne Walle.

## Step 1 - Preparation of the dataset
## Scraping comments from Youtube videos
In this stage, we have extracted Youtube comments from music video. The scraper python script is included.

## Step 2 - Loading and Pre-processing

## Load Dataset
Scraped video is loaded.

### Removing Irelevant Information
In this part usernames and URL's are removed.

### Remove Emojis
It is optional to remove or preserve emojis. In sentiment analysis it can be useful, but for this project simplicity it's removed. 

### Normalize Amharic Script Variations
This is important part as it helps to standardize the texts.

### Remove Punctuation and Numbers 
Punctuations don't usually help models understand meaning, so they're removed. Numbers often add noise unless we're doing price prediction and dates analysis.

### Tokenization (Basic space-based)
This helps the computer to understand the texts as it can't uderstand as a whole.

### Amharic Stop Word
This words appear often but does't have important meaning.

### basic Amharic Stemmer and Lemmatization
Stemmer part used to remove defined prefixes and suffixes. Lemmatization reduces words to their base or dictionary form(lemma). It is important to make different forms of the same word to be treated as the same. This technique is necessry for sentiment and classification.

## Step 3 - Feature Extraction Approaches
### Bag of Words (CountVectorizer)
### TF-IDF Vectorizer
### Word2Vec Embeddings (gensim)
 
## Step 4 - Sentiment Analysis Approaches
### Lexicon-Based Approach (Recommended for Amharic)
This would be a dictionary of Amharic words with their sentiment scores
Example structure: {'መልካም': 1, 'መጥፎ': -1, 'ደስታ': 1, ...}

Then sentiment is analyzed and sentiment graph and word cloud is generated.

## Course

Social Network Analysis

### NB:
1. After the sentimet analysis we must see how exactly every comment is classified as positive, neurtral or negative manually to see the efficiency of our work, as ambuigity in classification is a serious challenge in NLP specially in amharic language as NLP corpus dataset in largely isufficient and modules needed to be eveloped.
2. The video comment we used was selected because of it's large amount of comments in it, there is no any political interest in it.