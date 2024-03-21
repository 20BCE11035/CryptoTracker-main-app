# CryptoTracker-main-app
Problem Statement A flutter mobile application to load a cryptocurrency pair trading data. See the attached images for the app design.

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
