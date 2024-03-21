# CryptoTracker-main-app
Problem Statement 
A flutter mobile application to load a cryptocurrency pair trading data. See the attached images for the app design.

Problem Statement
A flutter mobile application to load a cryptocurrency pair trading data.
See the attached images for the app design.

API
Refer: https://www.bitstamp.net/api/
API to load data
GET https://www.bitstamp.net/api/v2/ticker/btcusd
API to load order book
GET https://www.bitstamp.net/api/v2/order_book/btcusd
Screens

Screen 1
------------
A screen for the user to enter the cryptocurrency pair to load data.

Supported values for currency pair: btcusd, btceur, btcgbp, btcpax, btcusdc, gbpusd, gbpeur, eurusd, xrpusd, xrpeur, xrpbtc, xrpgbp, xrppax, ltcusd, ltceur, ltcbtc, ltcgbp, ethusd, etheur, ethbtc, ethgbp, ethpax, ethusdc, bchusd, bcheur, bchbtc, bchgbp, paxusd, paxeur, paxgbp, xlmbtc, xlmusd, xlmeur, xlmgbp, linkusd, linkeur, linkgbp, linkbtc, linketh, omgusd, omgeur, omggbp, omgbtc, usdcusd, usdceur

Actions:
1. Clicking on the search icon will load the data

Screen 2
-----------
Display the tick data for the currency pair. Data to show include:
Name of the currency pair
Timestamp
Open Price
High Price
Low Price
Last Price
Volume

Actions:
1. A floating button to refresh the data
2. Show the Order Book button to load the order book

Screen 3
-----------
The order book expands inline to show the top 5 bid and ask price

Actions:
1. Hide Order Book button to hide the order book

Technical considerations

1. There should be a separation of concerns between views and data/logic.
2. Please ensure all best practices are adhered to while developing the Flutter app.
3. Unit & Widget testing is required.

<div align="center">

# CryptoTracker
</div>

**CryptoTracker is a discord bot made to display as much crypto currency pair prices as possible.**<br/>

# Installation
First of all you need to install Java 8.<br/>
Then you can drag and drop **"CryptoTracker.jar"** inside your folder of choice.<br/>

# Run
```
java -jar CryptoTracker.jar
```
You can also use a session manager to make your bot run 24h/24.<br/>
A good tool called tmux (only working on linux OS) -> https://tmuxcheatsheet.com/.<br/>

# Usage
Display is done automatically, though you can have a look at the bot's stats by using the command.<br/>
```
/stats
```

# Configuration
This is how the configuration looks like.<br/>

![](Showcase/config_default_exemple.png?raw=true "Default Config Exemple")
![](Showcase/config_custom_exemple.png?raw=true "Custom Config Exemple")

You have two exemples:
- on the left, the default configuration that you will have to fill up with your informations.<br/>
- on the right, a custom configuration (without bot token for security reasons).<br/>

The configuration is pretty self-explanatory:
* `token`: your bot token generated when creating an app on (https://discord.com/developers/applications).<br/>
* `symbol`: ***PAIR1*** is the crypto you want to track and ***PAIR2*** is it's reference price<br/> 
    -> (BTCUSDT) as an exemple means you are tracking BTC price according to the USDT price.<br/> 
* `crypto`: ***PAIR1*** is the crypto you want to track<br/> 
* `owner_id`: your personal id on discord (optional).<br/> 
* `decimal`: decimal displayed on the price. (refer to "Tracking Exemples").<br/> 
    -> **4** as an exemple means with pair ***BTCUSDT*** : "***6185***"<br/> 
    -> **1** as an exemple means with pair ***LTCUSDT*** : "***9***"<br/> 

# Tracking Exemples
Some exemples of configurations that can run.<br/>

![](Showcase/btc_exemple.png?raw=true "BTC/USDT Tracking Exemple")
![](Showcase/eth_exemple.png?raw=true "ETH/USDT Tracking Exemple")
![](Showcase/ltc_exemple.png?raw=true "LTC/USDT Tracking Exemple")

# Other information
Looking to get more details? Please refer to Binance API on (https://www.binance.com/en/binance-api).<br/>

# Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.<br/>
Please make sure to update tests as appropriate.<br/>

<img width="1225" alt="design" src="https://github.com/20BCE11035/CryptoTracker-main-app/assets/153983455/2abcc0d3-dac5-4853-bbdc-4dce5ebbb139">

