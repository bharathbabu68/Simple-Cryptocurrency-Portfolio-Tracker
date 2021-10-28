# Simple-Cryptocurrency-Portfolio-Tracker
This is just a pretty basic cryptocurrency portfolio tracker I made using the WazirX API using Python to track the status of cryptocurrency investments. The reason I made this was cause WazirX didn't provide a way to track the status of each coin that I owned, and didn't show individual details like profit amount, profit %, invested amount, but only showed the current value of the entire portfolio which made it really difficult to keep track of. 

## What do you get?
- You get to track the status of each coin you invested in, showing details such as prodit amount, profit %, invested amount and the current value of your investment. 
- Finally you also get the overall profit percentage of your portfolio, and the current value of all your investments. 
- I've also added a feature to get the realized profit for the coins you have sold. 

## How to Use It?
- Ok so, first you call the get_index function with the crypto you hold as a parameter, and this returns the index of the crypto in the JSON file that is returned. 
- Next, you go to crypto_to_index function and you put the crypto name you own followed by its index. for ex: 'btc':36. Basically crypto_to_index is a disctionary which maps the crypto to its index in the JSON file. 
- Next you add the crypto whose price you want to track to the cryptos list, which just holds the names of all cryptocurrencies that you own. 
- Correspondigly, you enter the price at which you bought the crypto onto the bought_prices list followed byt the quantity you bought onto the bought_qty list. 
- And that's it, you're good to go. 

## What I used to make this?
- I used the request library in Python to send a get request to the WazirX api site, which returns the data in the form of a JSON file. 
- I'm then storing the JSON indexes of whatever crypto I own, so that we don't need to fetch the details for each crypto one by one, you just fetch the entire thing and you can use the indexes to access all your cryptos. 
- I'm using the JSON library to load the content from the request into a JSON format. 
- For viewing my portfolio I'm just using a pandas dataframe and using red/green colors to differentiate between proditable and non-proditable investments. 

## How it Looks?
- So it looks something like this, once you've put in details related to your investments. Although my investments from the screenshot are not financial advice and crypto is really volatile and risky. So proceed with caution. 
![Crypto-Screenshot](https://github.com/bharathbabu68/Simple-Cryptocurrency-Portfolio-Tracker/blob/main/images/random_crypto.png)
