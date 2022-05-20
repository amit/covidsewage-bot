# covidsewage-bot

The [@testacc2013](https://twitter.com/testacc2013) Twitter bot

Tweets a daily image of the charts from the County of San Diego [SARS-CoV-2 Sewage Monitoring Data](https://sd-sequencing.info/wastewater).

This is a re-jig of Simon Willison's bot which does the same for Santa Clara County charts.
Background on this project: [Building a Covid sewage Twitter bot](https://simonwillison.net/2022/Apr/18/covid-sewage/)

## How it works

The bot runs using [this scheduled GitHub Actions workflow](https://github.com/simonw/covidsewage-bot/blob/main/.github/workflows/tweet.yml).

It uses these two tools:

- [shot-scraper](https://datasette.io/tools/shot-scraper) to take the screenshot
- [tweet-images](https://github.com/simonw/tweet-images) to send the tweet

I wrote notes on [how to get credentials for a Twitter bot](https://til.simonwillison.net/twitter/credentials-twitter-bot).
