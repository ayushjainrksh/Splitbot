# What's SplitBot?
SplitBot is a conversational chatbot using SplitWise API. Splitwise is a free tool for friends added in group on Zulip to track bills and other shared expenses, so that everyone can get their bills splited according to their share. Bot built using OAuth, flask, SplitWise API, Zulip API and other services.

# Features
Following use cases are supported by our bot
1. Show Friends
2. Add expense to the group that will be splited equally among all the members of the group.
3. Add expenses to a particular friend.
4. Show Balances after simplifying all the debts.

# How to set up the bot?
- Fork the repo.
- Clone the fork using : `git clone https://github.com/ayushjainrksh/Splitbot.git`
- Enter in the Splitbot directory: `cd Splitbot`
- Create a config.py file with the following content:
  1. consumer_key = 'Enter_here'
  2. consumer_secret = 'Enter_here'
  3. secret_key = 'test_secret_key'
- This can be obtained from splitwise API by registering your app.
- Create a zulip account.
- Create a bot from settings and download the zuliprc file.
- Set up zulip development server as instructed in https://zulipchat.com/api/running-bots.
- Open a terminal in Splitbot directory and run: `python app.py`
- Open another terminal in python-zulip-api directory and run start the bot with name splitbot and location of zuliprc file.
- Now visit your zulipchat account and tag the bot.
