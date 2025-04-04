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



## 2.Twitter Data extraction and sentiment analysis, then correlating it with market changes
using Selenium we are able to scrape thru live twitter tweets data and then save it into a file (also we have a keyword alert system in it, which alerts us on certain keywords that were found in scraped tweets data) , further we use VADER for analysing sentiment of our extracted tweets and then we save it in file, we then finally proceed to correlate this data agiainst live market price fluctuations (in sp500), on daily and hourly basis.


## 3. Market Sentiment Dashboard:
first merging all our data into a single file which contains the sentiment vs market change files for twitter and google news sentiment on hourly and daily basis, then using it to create visualizations and graphs using Plotly.

## 4. SEC fillings based Alerts:
using the API key from SEC Edgar we can access the sec earnings transcripts of any msjor company ny using their CIK code, so i extracted sec fillings of the top 50 by market cap s&p500 companies sec earning transcripts data, which amounted to almost 29000 trnascripts, then i ran a code which went through and found alerts in the sec fillings based on 1. the value of that filling, if it crosses a threshold (4.9 billion dollars here) it is marked as an alert as it is considered that such deals can signify major market movements 2. invalid negative values, these are marked as these could signify depper issues in our alert system in formatting certain data or some financial issue that needs deeper inspection

## 5. A Macro Data Analysis of current economy:
Using FRED api key i was able to extract data from their website on about 40 major economic indicators for the US economy, then saving that data in a file and using it for visulaizations using Plotly, showing how major macro eco indicators are correlated to each other on a heatmap. Then i proceed to include market data in this, showing how even the sp500 data is correlated with macoeconomic metrics, making also a scatter plot between the VIX and S&P500 monthly returns. Finally what we do with our obtained data is using the GDP data obtained from fred over the last 10 years, month over month, i use an ARIMA model to predict the future 8 months of GDP data and gain some key insights from statistical analysis of this data.

## Future Enhancements 
1.Enhancement in uding better sentiment analysis models like FinBert.
2.More smart scraping of data, so that false tweets or irrelevant social media data is not considered
3.Better models than ARIMA for predicting future changes in certain macro ecoonomic metrics

## Data Sources 
- **Google News RSS feed url for stock market data : "https://news.google.com/rss/search?q=stock+market&hl=en-US&gl=US&ceid=US:en"**
- **Twitter Scraping using Selenium and Chromedriver** (check your chrome-driver version properly)
- **SEC Filings: SEC EDGAR API key: https://www.sec.gov/search-filings/edgar-application-programming-interfaces** 
- **FRED APIs data: https://fred.stlouisfed.org/docs/api/api_key.html** 

## Required libraries: 
i will attach a requirements.txt file to this repository for that you can access it

## Contributors 
- **Krishna Barai** (Project Lead & Developer)
- [My github profile](https://github.com/HeroicKrishna160905) 

## License 
This project is private and not publicly distributed.

---
📌 *For any questions or access requests, contact the repository owner.*
(mail: krishnabarai160905@gmail.com/2024eeb052.krishna@students.iiests.ac.in)














