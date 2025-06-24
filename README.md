# Paarser-X

## About
Parser X is a Python-powered tool designed to automate the extraction and sentiment analysis of tweets from specific Twitter users. By combining web scraping techniques with natural language processing, Parser X enables users to collect, organize, and evaluate public Twitter data efficiently. It leverages the Twitter API for data access and VADER sentiment analysis for interpreting emotional tones in tweets.


**Core Features-**

1-Automated Tweet Collection
Fetches tweets for users listed in users.txt via Tweepy and stores them in individual .csv files.
2-User-Specific Organization
Creates a folder for each user containing their tweet data.
3-Sentiment Analysis
Applies VADER to classify tweets as positive, negative, or neutral.

Modular Scripts

twitter_tweets_parser.py: Fetch and save tweets
twitter_sentiment_analyzer.py: Analyze tweet sentiment

**Tech Stack**

1.Language: Python
2.Libraries: Tweepy, TwitterAPI, VADER
3.Formats: TXT, CSV, JSON
4.Config: config.py for API keys and parameters

**Use Cases**

1. Social media monitoring
2. Public sentiment tracking
3. Research and analytics
4. Data collection for ML/NLP

**Future Enhancements**

1. Real-time streaming
2. Sentiment visualization
3. Multilingual support
4. Database integration

## How to use it

1. Configure API Keys and Access Tokens in `config.py`(Don't share these with anyone)
2. Adjust additional params in `config.py`
3. Prepare a list of usernames in `users.txt`

### Tweets
1. `python twitter_tweets_parser.py`
2. For each user there will be created a folder named `{user_name}` with with `{user_name}_tweets.csv` file inside it.

### Account Data
1. `python twitter_account_data_parser.py`
2. For each user there will be created a folder named `{user_name}` with with `{user_name}_account_data.csv` file inside it.
3. There will also be a single `account_data.csv` file combining all entries in output folder.
