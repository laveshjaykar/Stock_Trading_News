# Stock News Notification System

This Python project provides a simple way to monitor significant changes in Microsoft's stock price (MSFT) and receive related news articles when certain thresholds are met. Utilizing the Alpha Vantage API for stock information and the NewsAPI for fetching relevant news articles, this script can be a handy tool for investors and enthusiasts interested in Microsoft's stock performance.

Features

Stock Price Monitoring: Monitors the closing price of Microsoft's stock (MSFT) and calculates the percentage change between the last two closing prices.
News Alerts: When the stock price change exceeds a specified threshold (e.g., 5%), the script fetches the top 3 news articles related to Microsoft and sends them via SMS.
Twilio Integration: Utilizes the Twilio API to send SMS alerts with the stock price change and related news headlines.
How It Works

Stock Price Change Calculation:
The script fetches daily stock data for Microsoft (MSFT) from the Alpha Vantage API.
It calculates the percentage difference in closing prices between the last two days.
News Article Retrieval:
If the stock price change exceeds the predefined threshold, the script queries the NewsAPI for the latest news articles that mention Microsoft in their titles.
It formats the top 3 articles, including their headlines and brief descriptions.
Sending Alerts:
The formatted news articles, along with the stock price change information, are sent as SMS messages through the Twilio API to a predefined recipient.
