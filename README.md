# Web Scraping: ebay-dl.py

## What does this do?

The [ebay-dl.py](https://github.com/NACB/ebay-dl/blob/main/ebay-dl.py) file allows a user to input via the terminal the name of an item they would like to search for on Ebay. It then returns a .json file containing key product information for the first 10 pages of results. This information consists of:
1. Product name, as shown in the item's listing
1. Whether or not the item has free returns
1. The number of each item already sold (if applicable)
1. The condition of the item (new, used, etc)
1. The price of each item (in cents)
1. The shipping cost of each item (in cents)

## How do I run it?

This file can be run via the terminal in VSCode by inputing
```
ebay-dl.py 'SEARCH TERM' --num_pages=X
```
wherein SEARCH TERM is the user desired search term and X is the user desired number of pages to be scraped. Without the `--num_pages=` flag, the program will default to 10. Below are three example searches and their results:

1. Search for zippo
```
python3 ebay-dl.py 'zippo'
```
[zippo.json](https://github.com/NACB/ebay-dl/blob/main/zippo.json)

2. Search for cocktail shakers
```
python3 ebay-dl.py 'cocktail shaker'
```
[cocktail shaker.json](https://github.com/NACB/ebay-dl/blob/main/cocktail%20shaker.json)

3. Search for big lebowski
```
python3 ebay-dl.py 'big lebowski'
```
[big lebowski.json](https://github.com/NACB/ebay-dl/blob/main/big%20lebowski.json)

### Why?
This program was created for a CS assignment. The assignment description can be found [here](https://github.com/mikeizbicki/cmc-csci040/tree/2021fall/hw_03).
