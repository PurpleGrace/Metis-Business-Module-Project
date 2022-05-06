## Recommendation For Real Estate investors in San Diego market based on EDA analysis
### Abstract
The ultimate goal of this project is to help identify properties worth investing for real estate investors of San Diego, California. We Hypothesis that through analysis of purchasing/selling transaction and renting records data, we can identify properties with good value growth potential or good rent to value ratio which indicates higher cash flow, thus we can provide reliable recommendation for the investors. Our initial analysis gives recommendations on zip code, house type and square footage range depends on if investors are seeking good value growth or higher cash flows. To have a more precise recommendation, our future work will be using linear regression model and machine learning methods to predict and forecast house value and rental value, we will also need more rental data which usually are available through purchasing from data company or big real estate platform companies.


### Design
During the covid_19 pandemic, many companies adopt policy which allows employees work from home and the trend is going to sustain even after the pandemic. Many family who live in bay area where the house pricing is hostile and severely unaffordable choose to move to San diego where house pricing is much more affordable, at the same time still stays in the State. Meanwhile, many real estate investors are actively purchasing rental properties due to the increasing inflation risk.As a result, San Diego house price increases 25% in a year and become one of hottest nationwide real estate market([source](https://www.sandiegouniontribune.com/business/real-estate/story/2021-07-27/san-diego-home-prices-now-up-25-in-a-year)).

However, there are near 20 cities and more than 80 zip code areas in the San Diego County, not to mention hundreds of neighborhoods and different kinds of property types. What area and what type of residential properties to invest become the first question to investors and buyers. Some investors look for good house value growth in the future, others may seek for higher cash flows. This project will identify properties with higher rental to value ratio or good value growth in the past years, thus to help investors make investment decisions based on data analysis evidence.


<details>
<summary>Impact hypothesis</summary>

We hypothesize that, int the future through EDA and more advanced machine learning model, the project can recognize the properties (combination with zip code, property type, square footage, and etc) with good investment potentials, so that investors can
-  make investment decisions based on solid scientific research result;
-  save time, energy and resource for market researching and make decisions in a timely manner;
- avoid loss due to lack of experience and knowledge about San Diego Real Estate market.

</details>



<details><summary>Solution Path</summary>
The **Technical** solution suggested to use in this project includes:

- Linear regression model to predict house value, so that investors can find properties with better rent_to_value ratio.
- Time series model to forecast future house value, so that investors to find properties with good value growth potentials.
- Clustering Algorithms to help find good substitutes when desired property type is not available on the market.

Other **Non-technical** solutions:
- Seek suggestions from experienced realtors or investors in the San Diego market;
- Utilizing common knowledge about real estate investment.

</details>

<details>
<summary>Measure of success

The metric keys in the project will be value growth rate and rent_to_value ratios.The model can be tested on test data to check that if recommended properties types have higher metric values. Also,In the long term, stakeholders can check if the model provides good recommendation for investment.
</summary>
</details>

<details><summary> Assumptions And Risks</summary>


|  Assumption    |   Risk    |
| :------------- | :------------- |
| To calculate the rent to value ratio, we need to estimate the value of rental property through analyzing/modeling purchasing transaction data. | The accuracies of estimation of rental property value depend on the accuracies of regression and machining learning models. |
| In our initial model, due to limited rental data, we assume location, house type and property size are three biggest elements for deciding property value. In the future work, we should use more features.  |Individual outliers will have big impact on the average rent_to_value ratio for a specific property combination, this should be resolved by complete rental data provided and more complicated features in the future.  |


</details>




### Data
San Diego purchasing and rental transaction records can be found in the Multiple Listing System(MLS).The data used in the project includes 30,000+ purchase transaction records in 2012 and 2021 respectively and around 2000 residential rent/lease records in 2021. Each record contains features like property geographic info, size, property type, age, bedroom numbers and etc.The rental records used in this initial project is limited, more and compete rental records should be able to purchased from data company or large real estate platforms, like Zillow or Redfin.


### Algorithms
The project use google sheet for data cleaning, calculating and pivot table. Tableau is used for visualizations.

To calculate the rent_to_value ratio for rental properties, we need to estimate the market value.The 2021 selling transaction data is used to fulfill the goal. We classify the properties into subcategories according to zip cods, property types and house size, calculate the average price/square feet and use the result to obtain the market value. Then we weight the rent_to_value ratio and DOMLS(days on market) to get a final ```Weighted recommend index```.

To find out what kind of properties have higher growth potential, we compared the price/square feet in 2012 and 2021 for property combinations (zip code, property type and square range) and recommend those with highest growth percentage.




### Tools
- Google sheet for data cleaning, aggregation and visualization
- Tableau for geographic and advanced data visualization

### Communications
A PPT presentation will be presented.
