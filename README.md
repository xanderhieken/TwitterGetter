# Using the Twitter API to Request and Stream Data

**This notebook illustrates three different methods of requesting Twitter data**

1. Using OAuth2 to pull data from Twitter's standard search API in JSON format

3. Using Tweepy to pull data from Twitter's standard search API into a SQLite database
 
5. Using Tweepy to pull live data from Twitter's streaming API in JSON format

## Prerequisites

Before you can request data from the Twitter API, you are going to need to create a Twitter account and generate your own keys on apps.twitter.com

```
API_KEY = 'INSERT YOUR KEY HERE' 
API_SECRET = 'INSERT YOUR KEY HERE'
TOKEN_KEY = 'INSERT YOUR KEY HERE'
TOKEN_SECRET = 'INSERT YOUR KEY HERE'
```

### Installing Dependencies

The packages necessary to run this notebook are provided in requirements.txt which can be installed using the following command in the terminal:

*Make sure requirements.txt is in the terminal's current directory*

```
pip install -r requirements.txt
```

## Running the Notebook

The first two methods illustrated in this notebook include a variable with a "hard coded" search term that can be replaced with **up to ten** words, hashtags (#example), and/or usernames (@example) that you want to request from Twitter's standard search API. 

The third method uses Twitter's streaming API, which uses the following format to enter your search term(s):

```
stream.filter(track=['ENTER YOUR SEARCH TERM(S) HERE'])
```

### Data Format

Twitter's standard search and streaming APIs will return data in JSON format.

The second method used in this notebook illustrates how to store and query that JSON data in a SQLite database. 

## Author

**Xander Hieken** - *Additional Work* - [xanderhieken](https://github.com/xanderhieken)


## Acknowledgments

* Jacqueline Kazil & Katharine Jarmul's book [Data Wrangling with Python](http://shop.oreilly.com/product/0636920032861.do)
