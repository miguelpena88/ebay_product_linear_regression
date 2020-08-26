
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

On this project I will be focusing on sale history of the Gameboy Color. I will be focusing on the following attributes to see if they play a role on the items fluctuating price:

```
    data = { 
        'title': title,
        'price': price,
        'currency':currency,
        'shipping':shipping,
        'date_time':date_time,
        'condition':condition,
        'location':location,
        'region_code':region_code,
        'color':color
    }
```

The following atrributes were scrapped using beatutifulsoup and regex libraries to access the ebay website. The entire dataset is stored in a csv file.

# Part 2: Exploratory Data Analysis

To determine the importance of each feature, I ran an exploratory data analsys looking at the distrubution of each feature. I used Tablau and matplotlib libraries to create my visualizations:

[image1]
[image2]
[image3]

# Part 3: Logistic Regression model

After running an EDA to get a better understanding of my data. I chose and engioneered the following key features to run on my logistic regressions model:


