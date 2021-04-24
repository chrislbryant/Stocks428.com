# Stocks428

### Go to [Stocks 428](https://www.stocks428.com/)

<br>
The goal of this project was to create an App allowing a user to create a price movement alert for US stocks and be notified via text message when the price rose above or below the user defined price. After successfully implementing the alert service, features to display stock charts, place trades, view orders, positions, balances, and a portfolio chart were added for a better user experience.

<br>
<br>

## App Design
<br>

This app uses <b>Python Django</b> with a <b>Postgres database</b>, <b>Javascript</b>, <b>HTML</b>, and <b>CSS</b>. In addition the following API’s and Libraries were used:


* <b>Twilio</b> – manage text messaging
* <b>Plotly</b> – charts
* <b>Polygon</b> – manage stock data
* <b>Alpaca</b> – manage stock trading
* <b>Django</b> – manage user account and profile 

<b>Django</b> is hosted on a Digital Ocean Droplet that is served with <b>Nginix</b> and <b>Gunicorn</b>. 

The <b>Postgres</b> database is located on a Digital Ocean Managed Database Server seperate from the webserver droplet.

The Messenger Script is located on the webserver droplet. A Chron job starts the srcipt every M-F at 4am. The script stops running at 8. The Messenger Script is responsible for checking alerts database table against a stocks current price (rises above or falls below) or the 52 week high/low. Once a users alert criteria are met a text message is sent to the user.

The website is compromised of the following pages:
* Home, Register, Login, Logout, Alerts, Alert History, Trade, Portfolio, and Profile

<br>

## Features:

Receive text messages when alert criteria is met and when placing trade orders.

Request real time data on any stock when placing an Alert.

<b>The Live chart is my favorite feature! The live chart displays the last 15 minutes in candlestick format and updates every market minute. Hovering over a bar shows the OHLC and V. Volume is also displayed visually with each candlestick.</b> 

Research charts include OHLC, Candlestick, and Close. These charts can be pulled based on user specified data making each chart custom to the user’s preferences. 

This platform allows the user to place trades using their Alpaca account. Users can use a paper or live trading account. Users can also view their positions, orders, and account balances.

Users can see their portfolio for a specified timeframe. (days, weeks, months, years)

<br>

The code for this app is in a private repository. I would be happy to demonstrate the code upon request.

### This app is deployed! Go to [Stocks 428](https://www.stocks428.com/) to create an account!

