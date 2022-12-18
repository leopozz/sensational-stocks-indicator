# Trend-Detecting-Indicator
Dear Reader, 

Before you can take advantage of our stock market indicator, we would like to tell you how this group of five guys organized themselves to accomplish this project. It all stemmed from our university course, "Introduction to Programming," where we were required to learn the basics of programming by developing something together with other classmates. Therefore, as finance enthusiasts, our team decided to focus on creating an extension for the TradingView site, which allows adding more indicators on all stock charts, forex, crypto, and etc.

First, we focused on a frequent problem of traders and tried to find possible help. Our indicator's mixture of the two modules can be advantageous for a trader. Moving averages help detect the trend direction of a stock and allow the trader to identify support and resistance levels on the chart. However, they usually provide this information to the trader in the timeframe they are looking for. This means that if, for instance, the chart is on 30-minute candles, the moving averages will show the trend, as well as support and resistances, for the 30-minute chart. This can be disadvantageous because the trader might receive short-term information but no long-term information. This can be best described by an example where a trader sees a bullish trend on the 30-minute chart while the daily chart shows a significant bearish trend. Therefore, our group decided to address this issue by providing the trader with moving averages based on the chart's timeframe and moving averages based on other timeframes so that the trader is no more biased by the lack of additional confirmation by other timeframes. Moreover, for the trader, it is more efficient to have all the information on one chart rather than constantly switching between different timeframes.

Each team member worked on a different task, between programming, code commentary, and implementation. Once the code was complete, we went through several rounds of review and debugging to ensure the indicator worked and minimized programming errors. Next, we focused on implementing the extension in TradingView. Once our extension is added to the site, you can choose any chart inherent in stocks, forex, and crypto, apply our indicators to simplify your strategy and get ready to make money. Have fun!

# Instructions-How to run our code:
Either from the Website: https://www.tradingview.com/chart/ or from the Desktop app, downloadable from: https://www.tradingview.com/desktop/
1. Click on the "Pine Editor" tab at the bottom of your TradingView chart ![Pine Editor on TradingView homescreen](https://user-images.githubusercontent.com/119878846/208310345-b82edf52-ad16-4ced-8206-4ed9fe38f8b5.png)
2. Select all code already in the editor and cancel it
3. Copy our code and paste it into the editor
4. Click "Save", choose a name and then click "Add to Chart"
5. The indicator will appear in a separate Pane under the chart
6. Make money!

For further information on how to use the Pine Editor, please visit: https://www.tradingview.com/pine-script-docs/en/v4/Quickstart_guide.html,
and use the User Manual

# Code content and structure:
As you can see, we divided the code into two different modules. The first module defines the three "chubby" averages (AVG1.1, AVG1.2, AVG1.3). Furthermore, in the first part, the three averages have a time frame that does not correspond to what the user decides on the chart (this will be done later in the second module), as the indicator aims to provide more confirmation signals to the user by including confirmations from other timeframes.
On the other hand, module 2 defines the three "thin" averages (AVG2.1, AVG2.2, AVG2.3). These averages are based on the timeframe selected by the user on the chart. Depending on the timeframe chosen by the user, the moving averages will adjust accordingly.

Focusing on the lines, the red line was called AVG1.1, the green AVG1.2, the blue AVG1.3, the orange AVG2.1, the lime AVG2.2, and the aqua AVG2.3. As can be seen from the code on line 94, whenever AVG1.2 crosses AVG1.3, the graph unfolds a yellow circle, which confirms a positive trend. This occurs because we have defined the length of the moving averages, and AVG1.2 has a length of 50, while AVG1.3 of 200. 

# Error handling: 
Please make sure that you:

• (if you're using the Desktop App) have an updated version of TradingView

• deleted the pre-set code in the editor before pasting our code

• copied the entire code

• clicked on "Add to chart" to view the strategy

If errors still persist, try deleting the entire script and starting anew the "Instructions, How to run our code" steps

# Group participants:
Fabio Baas, Federico Luca Emanuele Campi, Leonardo Pozzi, Mihnea Serbanoiu and Rémy Zuchuat

