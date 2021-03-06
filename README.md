Configuration:

Configuration is controlled through [settings.cfg](https://github.com/JSkally/WahTime/blob/master/settings.cfg) which must be in the same
directory as [bounty_bot.py](https://github.com/JSkally/WahTime/blob/master/bounty_bot.py).  Your Twitter Application ID tokens need to be
stored in this file to give the script permission to post status messages
on your Twitter account.  This section is required, so expect the bounty bot
script to throw errors if you don't include it.  The Stack Exchange OAuth
section is optional, but you may run into API throttling if you try to
run the script too often without it.

http://dev.twitter.com/apps/myappid
http://dev.twitter.com/apps/myappid/my_token

Example settings.cfg
```python
[Twitter OAuth]
CONSUMER_KEY: Your Consumer Key
CONSUMER_SECRET: Your Consumer Secret
ACCESS_TOKEN_KEY: Your Access Token Key
ACCESS_TOKEN_SECRET: Your Access Token Secret

[Stack Exchange OAuth]
KEY: Your Stack Exchange OAuth Key
```

Logging:

Status messages will be saved in a file named status.log in the same directory with bounty_bot.py.  The target window for bounty expiration, the status message posted to Twitter, and the bounty expiration time are all logged to this file.

Error messages will be saved in error.log.

Forked from: Bill Cruise
(Bill the Lizard on Stack Overflow, @lizardbill on Twitter)

Based on [BountyBot](https://github.com/BillCruise/BountyBot)
Dependencies: [tweepy](https://github.com/tweepy/tweepy), [Twitter API](https://dev.twitter.com/)
