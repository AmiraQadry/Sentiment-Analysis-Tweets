# Sentiment Analysis Tweets
![](https://9to5mac.com/wp-content/uploads/sites/6/2019/09/Twitter.jpg?quality=82&strip=all&w=1600)
This project aims to perform sentiment analysis on tweets using the `SentimentIntensityAnalyzer` from the Natural Language Toolkit (NLTK) library.

## Dataset

The project uses a dataset of [tweets](https://www.kaggle.com/datasets/dineshpiyasamara/sentiment-analysis-dataset/data) from Kaggle .

The file should have a column named "tweet" that contains the tweet text.

## Prerequisites

Make sure you have the following dependencies installed:

- Python (version 3.6 or higher)
- pandas
- nltk

## Usage

1. The script begins by importing the required libraries, such as `nltk` for natural language processing and `pandas` for data manipulation.
2. Then utilize the `nltk.download()` function to obtain the necessary NLTK resources (vader_lexicon).
3. Using `pd.read_csv()`, the CSV file containing the Twitter data is loaded into a pandas DataFrame.
4. The script will perform sentiment analysis on the tweets using the `SentimentIntensityAnalyzer`. It will add a new column named "sentiment_score" to the dataset, representing the sentiment score for each tweet.
5. Filter the DataFrame according to positive, negative, and neutral sentiments for analyzing the sentiment results. The console displays the sentiment distribution, which shows the proportion of neutral, positive, and negative tweets.
6. The updated dataset with sentiment scores will be saved as `sentiment_analysis_results.csv` in the project directory.
