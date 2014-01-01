BTC-E Autotrade
==============

This is a simple ruby script for automated trading on btc-e.com using the btce gem. Currently configured to run locally.

This script assumes that the market will always rise. It functions by:

1. Placing a buy order at the current bid (buy) price
2. Immediately creating a sell order at the current bid price + the profit margin you'd like to make


A lot of the code will probably make more sense after familiarizing yourself with the btce gem: https://github.com/cgore/ruby-btce.
Getting Started
---------------
1. Clone the repo to your hard drive.
2. Create a yml file called **btce-api-key.yml** and fill it in with the following format:

    `KEY: YOUR_BTCE_KEY`
    
    `SECRET: YOUR_BTCE_SECRET`
3. Run `gem install btce`
4. Overwrite the global variables in trade.rb to your liking (currency pair, amount, sleep, etc...)
4. Run `ruby trade.rb` to exectute the script indefinitely.
