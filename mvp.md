# Business Project MVP

## Recommendation For Real Estate investors in San Diego market based on EDA analysis

### Business opportunity
During the covid_19 pandemic, many companies adopt policy which allows employees work from home and the trend is going to sustain even after the pandemic. Many family who live in bay area where the house pricing is hostile and severely unaffortable choose to move to San diego where house pricing is much more affordable, at the same time still stays in the State. Meanwhile, many real estate investors are actively purchasing rental properties due to the increasing inflation risk.As a result, San Diego house price increases 25% in a year and become one of hottest nationwide real estate market([source](https://www.sandiegouniontribune.com/business/real-estate/story/2021-07-27/san-diego-home-prices-now-up-25-in-a-year)).
However, what area and what type of residential properties will have  good value growth and rental potential become the first question to investors and buyers.This business project will help investors/buyers make investment decisions based on data analysis evidence.

### Desired Business Impact
There are near 20 cities and more than 80 zip code area in the San Diego County, not to mention hundreds of neighborhoods and different kinds of property types. Individual investors or start up real estate investment companies usually need to spend a long time to get familiar the market, do investigation and research before making investment decisions. Our model will identify 5 types of properties (based on combination of zip code, property type, and square footage) which have highest rent_to_value ratio and with best liquidity (lowest days on market)

### Solution Path
San Diego purchasing and rental transaction records can be found in the Multiple Listing System(MLS).The data used in the model includes 30,000+ purchase transaction records  in 2012 and 2021 separately and around 2000 residential rental records in 2021. Each record contains features like property geographic info, size, property type, bedroom numbers and etc. With above mentioned data, the following analysis is possible:
- Linear regression model to predict house value, so that investors can find properties with better rent_to_value ratio.
- Time series model to forecast future house value, so that investors to find properties with good value growth potentials.
- Clustering Algorithms to help find good substitutes when desired property type is not available on the market.



<img src="https://github.com/PurpleGrace/Metis-Business-Module-Project/blob/main/MVP1.png" alt="DOML and rent_to_value based on zip code">

The plot shows that if research is done on zip code levels, darker yellow zip code area are those with short average days on market, which means the properties in those area are more populated and desired by renters, for example zip code 92020, 92067,92011 and etc. Vice versa.


<img src="https://github.com/PurpleGrace/Metis-Business-Module-Project/blob/main/mvp2.png" alt="DOML and rent_to_value based on zip code">

From above plot, we can see that townhome with size between 1000-1499 in zip code 92128 have the shortest days on the market of 6 days. Meanwhile, attached condo with size between square size between 500 and 999 in zip code is a good candidate for investors who seek for cash flows.


### Impact Hypothesis
Through EDA and future regression model, investors can recognize the properties (combination with zip code, property type, square footage, and etc) with good investment potentials, so that they can make a quick investment decision based on solid scientific research result.


### Assumptions And Risks
- The rental records are not complete in the MLS system, more and compete rental records should be able to purchased from data company or large real estate platforms, like Zillow or Redfin.
- The accuracies of rent_to_value and value growth rate depend on the accuracies of regression and machining learning models.
