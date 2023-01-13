# Class 17

**Web Scrape with Python in 4 minutes**

Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.

Important notes about web scraping:
- Read through the website’s Terms and Conditions to understand how you can legally use the data. Most sites prohibit you from using the data for commercial purposes.
- Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be blocked from the site as well.

The code below contains the entire set of code for web scraping the NY MTA turnstile data:
```python
# Import libraries
import requests
import urllib.request
import time
from bs4 import BeautifulSoup

# Set the URL you want to webscrape from
url = 'http://web.mta.info/developers/turnstile.html'

# Connect to the URL
response = requests.get(url)

# Parse HTML and save to BeautifulSoup object¶
soup = BeautifulSoup(response.text, "html.parser")

# To download the whole data set, let's do a for loop through all a tags
line_count = 1 #variable to track what line you are on
for one_a_tag in soup.findAll('a'):  #'a' tags are for links
    if line_count >= 36: #code for text files starts at line 36
        link = one_a_tag['href']
        download_url = 'http://web.mta.info/developers/'+ link
        urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:]) 
        time.sleep(1) #pause the code for a sec
    #add 1 for next line
    line_count +=1
```

**What is Web Scraping?**

Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites.[1] Web scraping software may directly access the World Wide Web using the Hypertext Transfer Protocol or a web browser. While web scraping can be done manually by a software user, the term typically refers to automated processes implemented using a bot or web crawler. It is a form of copying in which specific data is gathered and copied from the web, typically into a central local database or spreadsheet, for later retrieval or analysis.

**How to scrape websites without getting blocked**

Web spiders should ideally follow the robot.txt file for a website while scraping. It has specific rules for good behavior, such as how frequently you can scrape, which pages allow scraping, and which ones you can’t.

- Make the crawling slower, do not slam the server, treat websites nicely
- Do not follow the same crawling pattern
- Make requests through Proxies and rotate them as needed
- Rotate User Agents and corresponding HTTP Request Headers between requests
- Use a headless browser like Puppeteer, Selenium or Playwright
- Beware of Honey Pot Traps
- Check if Website is Changing Layouts
- Avoid scraping data behind a login
- Use Captcha Solving Services

references

[Web Scrape with Python in 4 minutes](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)

[What is Web Scraping?](https://en.wikipedia.org/wiki/Web_scraping)

[How to scrape websites without getting blocked](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)

[Track Amazon Prices](https://www.youtube.com/watch?v=Bg9r_yLk7VY&ab_channel=developedbyed)


<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)