# NYT Web Scraper

This scraper program is designed to retrieve articles from the New York Times website in two steps using the NY Times API and general web scraping techniques.

***Please note***: We can use web scraping to retrieve articles in the second phase because we have a digital subscription to the NY Times. Without a subscription, web scraping may violate the NY Times' terms of service. Please ensure that you have the appropriate permissions before using it.


## NY Times API
We use the NY Times API to retrieve articles metadata that the NY Times makes publicly available. This includes headline, lead_paragraph, author, publication date, etc. 
1. Sign up to https://developer.nytimes.com/ and get an API key
2. Retrieve article metadata and parse it in a pandas dataframe, including the URL of the article

## Web Scraping
After that, we use web scraping to retrieve the article text. We use the Selenium and BeautifulSoup libraries for this purpose.
1. Create a selenium Chrome driver and send the request 
2. Parse the html and obtain text data 
3. Add a column to the pandas dataframe that contains the entire text. 

The code was adapted starting from [this repository](https://github.com/brienna/coronavirus-news-analysis). 
