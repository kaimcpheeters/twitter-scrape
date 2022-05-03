# twitter-scrape
Twitter Scraping Example

Twitter query syntax documented here: https://github.com/igorbrigadir/twitter-advanced-search

Tweets are returned as snscrape.modules.twitter.Tweet objects.

    ```
    from twitter_scrape import get_tweets
    def main():
        query = 'lang:en -filter:images soccer'
        tweets = get_tweets(query, dt.datetime(2022,5,2,0), dt.datetime(2022,5,2,1))
        for tweet in tweets:
            print(f"{tweet.user.username} tweeted \n {tweet.content} \n")
    ```
