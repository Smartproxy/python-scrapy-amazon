# Python Scrapy Amazon Scraper
Scrape Amazon product listings utilising scrapy &amp; residential proxies

# Prerequisites
To get started with Scrapy you will first need to install it using methods provided in their documentation. [Check here for more information](https://docs.scrapy.org/en/latest/intro/install.html)

# Authentication & Proxy setup

### Once you have an active subscription you can find your credentials & proxy addresses in Dashboard > Residential > Proxy Setup

Navigate to settings.py in /amazon/amazon/ folder and modify the following lines to authenticate.

```
SMARTPROXY_USER = 'SPusername' ## Smartproxy Username (Sub-user)
SMARTPROXY_PASSWORD = 'SPpassword' ## Password for your user
SMARTPROXY_ENDPOINT = 'gate.smartproxy.com' ## Endpoint you'd like to use
SMARTPROXY_PORT = '7000' ## Port of the endpoint you are using.
```

# Running the scraper

Navigate to the project folder and run the following command

```
scrapy crawl amazon_search
```

# Results

Amazon search results will be saved in /amazon/data folder in a .csv format
