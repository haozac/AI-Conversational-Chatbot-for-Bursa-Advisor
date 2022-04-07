<h1 align='center'>Conversational Chatbot for Stock Market Price Information and Signals </h1>

## Disclaimer 
This repository is strictly for educational purpose only. People who use this source code for your stock analysis are advice to do your own research before taking any action in stock market. 

## Introduction

![alt text](https://github.com/haozac/Ai-Conversational-Chatbot-for-Bursa-Advisor/blob/main/Intro_image.jpg?raw=true)

This repository is a project to develop a Telegram bot that understands 'natural language' via Dialogflow to provide financial advices based on Bursa Malaysia listed firms. The telegram bot is integrating with Dialogflow, a natural language understanding platform used to design a conversational user interface into web application or related uses. Here I am integrating with Telegram Bot as Telegram provide the Bot function which is easy to use and deploy. 

The features of the telegram bot included: 
- Daily update of Bursa Malaysia Stock Exchange performance 
- Stock Screener 
- Stock Analysis 

## Information of Features 
### Daily update of Bursa Malaysia Stock Exchange performance 
The first feature is to provide the users some insights on how well is the Bursa Malaysia market doing, for the past month. Users can ask the questions "how is market/bursa doing today" for the bot to respond. Some steps are involved to make it happen.

- First, each of the stock name and stock code listed in Bursa Malaysia Stock Exchange are scrapped using Beautiful Soup from **[Malaysia Stock Business](https://www.malaysiastock.biz/Listed-Companies.aspx)**. And by defining some functions, all the stocks are divided into 13 sectors which are predefined by Bursa Malaysia. 

- After clustering of stocks is done, the monthly return of each stock is calcualted by getting the price data from yahoo finance, and average it group by the sector. Finally, the results will be showcasing in the telegram bot as below. 
![alt text](https://github.com/haozac/Ai-Conversational-Chatbot-for-Bursa-Advisor/blob/main/demo_sector.jpg?raw=true)

### Stock Screener 
Second feature is to screen all the stocks in Bursa Malaysia and give users a list of stock code that the bot think is the best to buy today. Users will need to insert some input, for example "which stock is good to buy today" for the telegram bot to react accordingly. Below are the example of the feature: 
![alt text](https://github.com/haozac/Ai-Conversational-Chatbot-for-Bursa-Advisor/blob/main/stock_screener.jpg?raw=true)

### Stock Analysis 
The last feature is to give users an insight of how this particular stock is doing right now. For example, the bot will tell users what is the trend of this stock for the past 3 months, is today a good signal to buy or sell the stock, and give you a overview stock chart with trend line and support/resistance line. Users will need to ask the bot which stock to analyse by inserting a stock code as an input for the telegram bot to showcase the analysis. The technical indicators for the stock analysis are
- Exponential Moving Average
- Relative Strength Index 
- Volume 

![alt text](https://github.com/haozac/Ai-Conversational-Chatbot-for-Bursa-Advisor/blob/main/stock_chart.png?raw=true)

An example of feedback from the bot is as below: 
![alt text](https://github.com/haozac/Ai-Conversational-Chatbot-for-Bursa-Advisor/blob/main/signal.jpg?raw=true)

## Future of Works 
Of course, this project doesn't stop here. Some future work will be done as my experience in trading and data science skills increase. Here are some examples of the future works will be included in next few months:
- Deploy this telegram bot in Heroku apps and make it to public use as currently it is only available to run locally
- Add more feature into the telegram bot (forecasting of stock, algo trading using telegram bot)
- Include more exchanges


