### dtechbuild2025ds (Duke's DTECH Build Data Science Project)
# Sentiment Analysis of Meta: Do News Articles Influence Stock Prices?
## Created by: Fehintoluwa Benson, Sophia Sang, and Alexis Fox


## Overview
This project set out to explore a fundamental question in financial media analysis: Does the sentiment and volume of news coverage influence the stock price of a major company like Meta? 
The team specifically investigated whether daily changes in Meta’s stock price from 2023 to 2024 could be predicted using the number of articles written about the company and the sentiment
expressed in those articles.

## Modeling 
The approach combined data science with real-time news analysis. Using Python and the Pandas library, stock market data was first cleaned and processed. Dates were converted into a uniform format, null values were removed, and column names were standardized for easier analysis. The data was sorted chronologically to ensure consistency for time series modeling.

To assess media coverage, the team employed the GDELT (Global Database of Events, Language, and Tone) API. This tool aggregates news articles from across the web and provides sentiment scores based on the emotional tone of the text. The team filtered the results to include only articles where Meta was the main subject and where the sources came from prominent news platforms. Sentiment scores and article counts were collected for each day in the 2023–2024 timeframe.
