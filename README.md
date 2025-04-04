# market-sentiment-analysis-project
## Overview
This project aims to create a **Market Sentiment and Condition Analyzer** to help **traders and businesses** gather useful insights about the market. 

We start by analyzing the **correlation between real-time market price changes and sentiment data** from **news sources and social media**. Additionally, we generate **alerts from keyword data** collected from various sources to track how frequently certain market-moving terms appear.

Next, we incorporate **SEC earnings call transcripts** to analyze financial statements and detect potential indicators of upcoming market movements. Finally, we gather **macroeconomic data** from the **FRED website** to assess the overall economic condition and provide a deeper understanding of market health.

## Features
## 1.Google News Extraction and Sentiment Analysis against Market Price fluctuations and Correlation:
 using scraping technique (parsing the google news rss feed) we extract data from top financial sources articles like bloomberg and others,
 analyse their headings and apply sentiment analysisng function with help of Nltk library in python on them after cleaning the data,
 save the sentiment data in a file,
 we proceed to plot sentiment vs live market price changes (in s&p500) based on hourly and daily sentiments across those time periods.

 ![1styearproject - Google Chrome 30-03-2025 17_06_27](https://github.com/user-attachments/assets/eb22f56c-2969-493a-8efb-ac1fe93457f9)
Scraped tweet data and in-built keyword based ALert system

## 2.Twitter Data extraction and sentiment analysis, then correlating it with market changes
using Selenium we are able to scrape thru live twitter tweets data and then save it into a file (also we have a keyword alert system in it, which alerts us on certain keywords that were found in scraped tweets data) , further we use VADER for analysing sentiment of our extracted tweets and then we save it in file, we then finally proceed to correlate this data agiainst live market price fluctuations (in sp500), on daily and hourly basis.

## 3. Market Sentiment Dashboard:



















