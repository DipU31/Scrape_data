# Scrape_data
Scrape and extract products details from "Amazon.com" search results pages and return it in JSON format.

# Setting up your computer for web scraper development
We will use Python 3 for this Amazon scraper. The code will not run if you are using Python 2.7. To start, you need a PIP installed in it.

# How To Install Python Packages for Web Scraping in Windows 10
Install Packages
1. Python Requests, to make requests and download the HTML content of the Amazon product pages
2. SelectorLib python package to extract data using the YAML file we created from the webpages we download

Using pip3,
pip3 install requests requests selectorlib

# Markup the data fields using Selectorlib
Selectorlib is a combination of tools for developers that makes marking up and extracting data from web pages easy. 
The Selectorlib Chrome Extension lets you mark data that you need to extract, and creates the CSS Selectors or XPaths needed to extract that data. 
Save this as a file as selectors.yml in the same directory as our code.

# The Code
Create a folder called amazon-scraper and paste your selectorlib yaml file as search_results.yml.
we iterate through each product and save them as a separate line.
Then create a file called searchresults.py and paste the code below into it. All it does is
1. Open a file called search_results_urls.txt and read search result page URLs
2. Scrape the data
3. Save to a JSON Lines file called search_results_output.jsonl

# Running the Search Result Scraper
You can start your scraper by typing the command:
python3 searchresults.py

Once the scrape is complete you should see a file called search_results_output.jsonl with your data.

Here is an example for the URL
https://www.amazon.com/s?k=laptops

