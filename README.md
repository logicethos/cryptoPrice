=cryptoPrice
-----------

**Google Spreadsheets coinmarketcap.com cryptocurrency prices** 
By Stuart Johnson, Logic Ethos Ltd


**To Install:**

Copy and paste cryptoPrice.gs into the Google Spreadsheet Script Editor.
Set up two triggers for "cryptoUpdateSheet".

 1. Time driven every 5+ minutes 
 2. On opening the document.

**To use:**

    =cryptoPrice(<coin>[,currency][,timestamp location])
    
    coin = "Ethereum","Factom","Bitcoin",.......
    currency = "USD,"GBP","EUR",......
    timestamp (cell) location = "left","right","top","bottom"

**Example:**

    =cryptoPrice("ethereum")
    =cryptoPrice("ethereum","GBP")
    =cryptoPrice("ethereum","GBP","left")

 
Set cell formatting for currency, and TimeStamp fields. 


**Notes:**
Updating the price too frequently generates errors over a 24h period (i.e setting it for every minute, with multiple prices).
The Date and Time is sent by CoinMarketCap, to show when the price was last updated.
