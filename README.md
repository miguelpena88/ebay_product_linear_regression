
# ebay Asking Price Linear Regression Project
A project based on the regression analysis of a single item’s sale history to predict its current asking price.

Ebay can be daunting. It is this “wild wild west”, meets the show “storage wars' ', kind of a marketplace; by this i mean... there are definitely moving parts at play. You want to make sure the item you are looking to buy is in the condition you expect--so be cautious!--but at the same time you don’t want to miss out on a great opportunity(or equally as bad, get lost in a bidding war.)

To help me navigate through this dynamic marketplace, I decided to scrape sales data from the ebay.com website and use a predictive model; thus adding palpable tools to this seemingly elusive process. I hope to improve the buy/sell decisions on the ebay marketplace for any target item,

This project will be split into 4 parts:

1. Obtain item sold listings data by scraping from the ebay.com website
2. Consolidate the data into a pandas dataframe
3. Perform exploratory data analysis (EDA) on the dataframe to find any relevant patterns and characteristics to the regression
4. Perform regression analysis on data gathered from the item’s sold listings

# Part 1: Obtain the data

I web-scraped ebay.com for a single item’s “available” sale history. Ebay keeps records of sold listings for up to 90days, so it’s better for our tests to pick a popular item with many sold listings. The search result lists fifty postings per page by most recent postings first. Each individual listing contains a url to the specific posting site, the sell price,  the color, condition, the unit number, the region, sell tome, and title of listing.
