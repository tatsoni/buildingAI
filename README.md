# Gaining the market - short term investing

Final project for the Building AI course

## Summary

Legendary value investor Benjamin Graham said “In the short run, the market is a voting machine but in the long run, it is a weighing machine.”, which has been understanded meaning that in short term popularity of the stock is what drives to price, but in the long run fundamentals under the stock are what drives the price. This has been followed be the great oracle of Omaha, Warren Buffett to great success and it is really good investment advice for regular investors. 

But if we just look at the first part of the quote "“In the short run, the market is a voting machine" and try to take advance of that.


## Background

With people talking about stocks, their investments and hyping certain stocks in internet we could see certain patterns in stock prices, for example GME which was hyped to record prices by internet, there are other examples that social media, discussion forums, etc hype has caused big spikes on stock price, like Tanger Factory Outlets Centers and Aphria. Predicting those possible spikes could be really useful for short term investing.

For data, easiest source for data could be reddit forums /r/wallstreetbets, /r/stocks, /r/weedstocks, etc. Finding stock info in twitter, instagram or facebook would be little more diffucult because of the amount of posts / data that is not relevant for stock prices, but it could be doable.

For the company stock data there are multiple possible sources, for example yahoo finance, where this data can be gathered. In this case the company business fundamentals would not be that interesting info, but instead data on how much stock is traded (volume), market cap, how much shorting is there for the stock, etc, so more data on actual stock and market, not the business. Also of course the result we want to see, the price change of the stock. As the stock market reactions are not instant and it would not useful buy and sell one hour later after 0,1% change, the stock price change should be one day or even week after the post.

First we would need to process the posts from reddit forums and see if the post would be positive (buy), negative (sell) and maybe neutral (hold) and how many likes, replies, if what the reply would be and likes on replies it would get to see how popular the stock is and to see if the hype is positive or neutral. For this we can use same methods as looking for spam emails. So Naive Bayes system can be teached to see if the post is positive, neutral or negative and then adding popularity info on it (likes, replies). We also need to consider that neutral post (hold) can be seen as little bit positive, for people considering buying that stock.

Combining this information with stocks market data we would have different data points and then getting the result, change of the stock price we would have data that you can use to predict if investing to the stock would be profitable. For this some regression model logistic or linear could be used.

Challenges for this is getting enough source data from people posting, as 100 people like the post and then maybe 10 of them buys that stock, that does not affect stock prices enough. The amount of hype that is needed to spike up the price is really big. 

This also could have negative impacts for investing as "first in, first out" are the ones that could be the only ones gaining big profits and the last people holding the bag could be quite big losers. But if the model would allow long term predictions it could help to see when the hype is dying and tell when stock could be sold before the prices starts to go down.

Also this would not work for long term investors as Graham said "but in the long run, it is a weighing machine." Hype will die down some point and the fundamentals will take over.

Future improvements would be adding more data sources like twitter to get better understanding of the popularity of the stock and analyzing the delay of the hype to when stock prices would react to that. Also adding data if the hype is growing and dieing down as data point.





