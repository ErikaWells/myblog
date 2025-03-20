---
layout: post
title:  "Sole Searching: Unveiling Sneaker Trends with Web Scraping"
author: Erika Wells
description: "Using GOAT.com to check out what I should be rocking in March 2025."
image: "/assets/images/Shoe_Header.png"  
---


# More Than Just Shoes
Sneakers are more than just footwear, they’re a cultural phenomenon! Whether it’s the latest Air Jordan drop or a nostalgic re-release, sneaker prices and demand fluctuate based on various factors like release date, hype, and exclusivity. In this project, I used web-scraping to collect data from GOAT, a popular sneaker marketplace, to analyze trends in sneaker rankings, prices, and release dates.


![Sneakers by Joshua Renfroe]({{ site.url }}/{{ site.baseurl }}/assets/images/sneakerhead.jpg)

<a href="https://www.instagram.com/joshuarenfroe_/?hl=en" target="_blank" rel="noopener noreferrer">Image by Joshua Renfroe</a>


## Chasing Trends: What Makes a Sneaker a Hit?
Every sneaker tells a story, but what makes some more valuable than others? This project explores:
- The relationship between sneaker rankings, prices, and release years
- Whether new releases outperform older classics
- Which brands and styles dominate resale rankings (coming soon)
- The most popular colorways right now (coming soon)


## Ethical Considerations & Web Scraping Best Practices
Before collecting data, I ensured that my scraping practices were ethical and aligned with best practices:
1. **Checking GOAT’s Terms of Service**: I reviewed GOAT’s website policies to confirm that automated scraping was permissible. Since GOAT does not provide an open API, I limited my requests to avoid server overload.
2. **Respecting Rate Limits**: I included a delay between requests to prevent overwhelming the site.
3. **User-Agent Header**: I set a user-agent in my request headers to mimic a real browser, reducing the risk of being blocked.
4. **Data Usage**: My goal was to analyze publicly available sneaker listings for educational purposes only, without redistributing or monetizing the data.


## How to Get the Data
For anyone interested in conducting a similar project, here is a breakdown of the web-scraping steps:
1. **Identify the Target Website**: Choose a reliable source like GOAT that provides structured data. I wanted to pick a site that included information of trends, specifically in fashion. This site worked perfectly because the sneakers were already ranked by most popular to least popular.  
2. **Inspect the Website Structure**: Use browser developer tools (F12 in Chrome) to inspect HTML elements containing product details. You'll come back to this step over and over again as you workshop your code. 
3. **Use Python for Web Scraping**:
   - `requests` to send HTTP requests
   - `BeautifulSoup` to parse HTML and extract relevant information
   - `Selenium` to pull dynamic data
4. **Extract Relevant Features**: I focused on key attributes such as rank, shoe name, price, release date, product link, and am currently working on getting main color and category.
5. **Store Data in a Pandas DataFrame**: This allows for easy analysis and visualization.
6. **Save Data for Future Use**: Export as a CSV for further exploration.


**If you want more than just a summary check out my code on Github** <a href="https://github.com/ErikaWells/ShoeAnalysis" target="_blank" rel="noopener noreferrer">here!</a>

## Summary of the Dataset
My final dataset includes:
- **182 sneakers**
- **Features:** Rank, shoe name, price, release date, product link, main color (if available), and category (if available)
- **Missing Data:** Some entries lacked information on color and category, which I'm currently working on adding by following each individual product link, stay tuned for new data soon!


## Interesting Initial Findings
While I will cover detailed Exploratory Data Analysis (EDA) separately, some initial observations include:
- A wide range of prices from $50 to almost $500!
- An average sneaker price of $156.58
- The majority of sneakers between $110.25 and $189.75

![Sneaker Prices]({{ site.url }}/{{ site.baseurl }}/assets/images/sneaker_prices_updated.png)

## Keep Learning
For those looking to replicate or push this project further, here are a few helpful resources:
- **Python Libraries**: <a href="https://docs.python-requests.org/en/latest/" target="_blank" rel="noopener noreferrer">`requests`</a>, <a href="https://www.crummy.com/software/BeautifulSoup/" target="_blank" rel="noopener noreferrer">`BeautifulSoup`</a>, <a href="https://pypi.org/project/selenium/" target="_blank" rel="noopener noreferrer">`Selenium`</a>
- **Web Scraping Guidelines**: <a href="https://docs.scrapy.org/en/latest/" target="_blank" rel="noopener noreferrer">Scrapy Documentation</a>
- **Sneaker Market Insights**: <a href="https://www.goat.com/sneakers/top-100" target="_blank" rel="noopener noreferrer"> GOAT Top 100</a>


### Access the Code
Here's another reminder that you can check out my full code and dataset in my <a href="https://github.com/ErikaWells/ShoeAnalysis" target="_blank" rel="noopener noreferrer">Github Repo</a>.


By following these steps, anyone can gain fun insights to their favorite brands top sellers AND learn a ton about data collection, web-scraping, and simple analysis. 
