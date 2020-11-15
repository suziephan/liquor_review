# BC Beer Recommendation (On-going)

## Project Summary
Beers go great with food. Beers may benefit your health. There are many reasons why you should have some beer once in a while, but if you are not a beer drinker, you might be overwhelm about the number of beers out there. As non-drinkers ourselves, we understand the struggle of going inside a liquor store, standing in front of a shelf, and spending minutes just to figure our what to buy. This project was built to help people with the same problem. We scraped the reviews from a beer review website of every beer product in BC Liquor Store, and recategorized all products based on taste and aroma. We recategorized this way because non-drinkers mostly care about these attributes. Since they do not know much about beer styles, it is not reasonable to categorize products into styles such as Ale, Lager, Wheat, etc. 

## Dataset
- All beer products scraped from [BC Liquor Store](https://www.bcliquorstores.com/product-catalogue?category=beer&sort=name.raw:asc&page=1).
- Reviews of these products scraped from [BeerAdvocate](https://www.beeradvocate.com/beer/top-rated/ca/bc/)

## Process
1. Scrape data
- From BC Liquor Store
- From BeerAdvocate
2. Categorize beers based on BeerAdvocate reviews
3. Fuzzy Matching Beer Name

## Obstacles & Limitations
1. BeerAdvocate requires log-in to see all reviews. Therefore a function has to be made to scrape these reviews.
2. The beer names from BC Liquor Stores and BeerAdvocate are not totally the same, which yielded incorrect results when we tried to use simple matching function. Fuzzy matching was then considered to match strings with some similar words.  

## Tools used
- Data Manipulation: Pandas/ Numpy
- Web Scrape: BeautifulSoup, Selenium
- Text Analysis: NLTK, TextBlob, Wordninja

## Timeline
15/09/2020 - now
