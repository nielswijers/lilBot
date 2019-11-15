# 'lil Bot
## The littlest crypto bot

Don't you wish you could use TrandingView charts, strategies and indicators to trade REAL crypto? You can! Using TradingView alerts. When an alert is triggered on your chart a webhook contacts this app.js script and tells it to place a buy/sell market order on the binance exchange. 

## Requirements:

### Clone this repo

[Download](https://github.com/modster/lilBot) 
Extract it to a convenient location.

### Binance Trading Account

Log in and create a new key. Beginners should disable withrawls and restrict access to your device's external ip. 
[API key](https://www.binance.com/en/support/articles/360002502072)

### NodeJS 

[Download](https://nodejs.org/en/download)

### Ngrok  

Sign up for an account and follow the instructions. Ngrok should be in the same folder as app.js.
[Download](https://ngrok.com/download)

**Important:** The ngrok.exe must reside in the same folder as app.js.

## TradingView Charts 

This is the only resource that isn't free. To use webhooks we need TradingView **Pro** ($10.95/month).
[Get a $30 credit by visiting this affiliate link](https://www.tradingview.com/gopro/?share_your_love=Greeffer)

## Create a new bot:

After the pre-requisits are installed open a terminal in the cloned repository and run the following commands:

``` bash
npm init -y

npm install node-binance-api --save
```

## Start:

To start run the following in your terminal.

``` bash

./ngrok http 80

node app.js
```

## Tips

Ngrok changes your url on startup, so you'll have to copy/paste the new url into your TradingView webhooks. Upgrade to ngrok pro to solve this. Don't forget to create an [auth token](https://ngrok.com/docs#getting-started-authtoken)

For testing webhooks go to http://localhost:4040 and select "replay". You can feed your bot any 
value you want without having to wait for your alerts to be triggered. 

To use the example bollinger ribbon pine script just copy/paste it into the tradingview pine editor at the bottom of your chart. By clicking 'new' a drop down menu displays many default scripts you can easily clone and edit to create your own custom indicators.
