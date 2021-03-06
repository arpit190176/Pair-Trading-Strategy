# Pair-Trading-Strategy
Summer 2021 project under Finance &amp; Analytics Club, IIT Kanpur

Pairs trading is a strategy in which we use various statistical methods to  pair-up 2 stocks whose prices have moved together in the past and are potentially market neutral. We monitor the spread between the prices and when these prices diverge, we short the winner and buy the loser. The paper can be read from [here](https://www.researchgate.net/publication/227624374_Pairs_Trading).

![alt](./images/pair.jpeg)
 ![image](https://user-images.githubusercontent.com/82868238/126040677-35d3f9be-fc31-40eb-80f2-1b68bc45ed4f.png)


There are two approaches:
## Distance Approach
The approach was proposed in a research paper  by Gatev et al.
In simple words the distance approach is when two stock prices are taken to see if they’re moving together based on a simple metric like a simple Euclidean distance. Then the spread of these two prices is calculated during the trading period and if it diverges greatly we just TRADE!!

## Cointegration Approach
Cointegration is a statistical property of a collection of time series variables which allow dynamic modelling of non stationary time series sharing a common stochastic trend. To check whether the given pair is cointegrated or not,  we can employ hypothesis testing. We form a null hypothesis that there is no cointegration, the alternative hypothesis is that there is cointegrating relationship. For that purpose we have to look at the p-value. A smaller p-value means that there is stronger evidence in favor of the alternative hypothesis.To find out the p-value we used a python library called “statsmodels“.

Link to documentation-https://docs.google.com/document/d/1VrZbQa7RTxDzQj3BdIVJvgFDeIis3Yc6k-vnjyuxJYc/edit
