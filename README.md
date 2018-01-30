# Crypto Market Watcher

A nodejs application to watch Cryptocurrency exchanges for the price of BTC/USD pair. Cryptocurreny exchanges used here are BitFinex, OKCoin and GDAX.


## Running the Application


```bash

# make sure you're in the project's directory
cd crypto-market-watcher

# Connect your mongodb database
./config/database.js
The default database url is 'url' : 'mongodb://localhost/test'

# installs project dependencies
npm install

# starts the server
DEBUG=crypto-market-watcher:* npm start
```

Visit [http://localhost:3000](http://localhost:3000) to view the application.

## Problem Description

You have been approached by a client who has a healthy interest in Cryptocurrency. He wants to know how the various coins are performing against US Dollars. His Company is mostly interested in Bitcoin. What his team needs is a dashboard that shows the price of Bitcoin at any point in time without having to refresh the browser. They need the pricing information in realtime because that'd influence their decision whether to buy or sell.

### Basic Features

* Improved UI/UX
* Sign up for users at your Client's company
* Login (you are free to use a package such as [Passport](https://www.npmjs.com/package/passport) for Authentication)
* Integration with at least 3 exchanges (with Websocket API for their market data). Examples of such exchanges are Bitstamp, OKCoin, etc.

### Advanced Features

Not yet available

* Persist the market data in a PostgreSQL database ([node-postgres](https://github.com/brianc/node-postgres))
* Allow users to set up alerts for a certain price point