 dtechbuild2025ds (Duke's DTECH Build Data Science Project)



# Sentiment Analysis of Meta: Do News Articles Influence Stock Prices?
Created by: Fehintoluwa Benson, Sophia Sang, and Alexis Fox


## Overview

This project set out to explore a fundamental question in financial media analysis: Does the sentiment and volume of news coverage influence the stock price of a major company like Meta? 
The team specifically investigated whether daily changes in Meta’s stock price from 2023 to 2024 could be predicted using the number of articles written about the company and the sentiment
expressed in those articles.

## Modeling 

The approach combined data science with real-time news analysis. Using Python and the Pandas library, stock market data was first cleaned and processed. Dates were converted into a uniform format, null values were removed, and column names were standardized for easier analysis. The data was sorted chronologically to ensure consistency for time series modeling.

To assess media coverage, the team employed the GDELT (Global Database of Events, Language, and Tone) API. This tool aggregates news articles from across the web and provides sentiment scores based on the emotional tone of the text. The team filtered the results to include only articles where Meta was the main subject and where the sources came from prominent news platforms. Sentiment scores and article counts were collected for each day in the 2023–2024 timeframe.


## Analysis 

The analysis then focused on building a simple linear regression model. Rather than predicting the absolute stock price—which trends upward over time—the model focused on the daily price delta, or the difference between the opening and closing stock prices each day. The two predictors used in the model were the average sentiment score for articles on that day and the total number of articles published.

To explore the relationships visually and statistically, the team plotted several key comparisons. The Meta stock price over time clearly showed an overall increasing trend, with some periods of volatility. Overlaying the article count on this timeline suggested that large spikes in the number of articles about Meta were often followed by significant daily price changes, especially during high-news-volume periods.

Further scatter plot analyses examined how the daily price delta correlated with article count and average sentiment. The data showed some clustering and occasional outliers, where unusually high article counts or extreme sentiment values corresponded with price jumps or drops. However, these patterns were not consistent enough to draw strong conclusions.

The linear regression analysis confirmed this ambiguity. Although there was some positive correlation between the media variables and daily stock price change, the correlation coefficient was only 0.4. This indicates a weak-to-moderate relationship at best, falling short of the threshold needed to confidently use sentiment and article count as predictive tools for stock movements.

## Conclusions and Limitations

In conclusion, the project provided partial support for the idea that media sentiment and volume might influence stock behavior, particularly on volatile days. However, the findings also highlight the complexity of stock market dynamics and the limited predictive power of media data alone. Sentiment and article count may be contributing factors, but they are far from definitive indicators of daily price direction.
