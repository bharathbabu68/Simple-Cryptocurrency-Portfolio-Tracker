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
