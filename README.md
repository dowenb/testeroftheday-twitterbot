# testeroftheday-twitterbot

Tester of The Day Twitter Bot - Retweeting  Hash tag TesterOfTheDay

## References

Followed guide:

<https://dev.to/sumedhpatkar/how-i-created-a-twitter-bot-using-node-js-and-heroku-368b#create-app>

And is a a modified clone of:
<https://github.com/Sumedh-Patkar/the-datascience-bot>

## Expected Behavior

* Will run once then exit
* Scheduled to execute once every 10 minutes via Heroku Schedular
* Should not send duplicate re-tweets
* Is a 'Worker' only and has no front-end

## Environment Variables

To run locally you will need a .env file with appropriate Twitter keys, in this format:

```Text
CONSUMER_KEY=XXX
CONSUMER_SECRET=XXX
ACCESS_TOKEN=XXX
ACCESS_TOKEN_SECRET=XXX
```

To run on Heroku, you will need to setup Config Vars, see the Heroku Docs:
<https://devcenter.heroku.com/articles/config-vars>

Remember to setup the keys exactly as above, including the uppercase and underscores.

## One of run

A single execution can be run locally by running:

```Text
node bot.js
```

A single execution can be run on heroku by running:

```Text
heroku run node bot.js --app testeroftheday-twitterbot
```

If you have forked this project, replace 'testeroftheday-twitterbot' with the name of your Heroku app.
Otherwise these are notes for me.
