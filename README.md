Download Link: https://assignmentchef.com/product/solved-cop4814-assignment-3-stock-price-observer
<br>
5/5 - (5 votes)

Using a stock portfolio model, design interfaces and classes that implement the Observer Pattern. Be sure to read Chapter 2 in Head-First Design Pattems first. A typical stock portfolio contains a collection of investments, and online brokerages let you view your investments in an application that periodically updates the display to reflect changing stock prices. Your program will write to standard output. You will probably need to build the program in steps:



. Create an Observer interface with a method that receives a Map of ticker symbols and prices.

2. Copy the Subject and DisplayElement interfaces from Chapter 2 with no changes.

3.  Create a PriceData class that is more or less like the WeatherData class in Chapter 2.

Rather than containing temperature, humidity, and pressure, this class should contain a Map of ticker symbols and stock prices. Make other changes to the class that seem appropriate.

4.  Create a PricesDispIay class that implements the Observer and DisplayElement interfaces. PricesDisplay contains a list of ticker symbols (as strings). It is much like the CurrentConditionsDispIay class from Chapter 2. Its Display method should display each ticker symbol and price for each stock in its list of stocks. To do this, it will need to get the prices from the prices map. This class operates as your logical stock portfolio, meaning that you will not define an actual Portfolio class.

5. Download and use the StockObserverTest class from my faculty website

<a href="http://users.cis.fiu.edu/%E2%80%94crahn/" target="_blank" rel="nofollow noopener">http://users.cis.fiu.edu/—crahn/</a> which creates the necessary objects and simulates the changes in stock prices. Each time it changes the prices, it calls a method in the PriceData class that broadcasts the new prices to all observer objects. The program’s output will resemble the following, where the two observer objects (one for each portfolio) have received a series of stock price updates and displays the information on the screen in pairs with a blank line between them as follows:

Each portfolio contains a different list of stocks.