**Exploring Sneaker Trends with Web Scraping**


### Introduction
Sneakers are more than just footwear, they’re a cultural phenomenon. Whether it’s the latest Air Jordan drop or a nostalgic re-release, sneaker prices and demand fluctuate based on various factors like release date, hype, and exclusivity. In this project, I used web scraping to collect data from GOAT, a popular sneaker marketplace, to analyze trends in sneaker rankings, prices, and release dates.


### Motivating Question
The goal of this project was to explore patterns in sneaker popularity and pricing. Specifically, I wanted to investigate:
- How do sneaker rankings correlate with price and release year?
- Are newer releases consistently ranked higher than older ones?
- Which brands or categories dominate the top rankings?


### Ethical Considerations & Web Scraping Best Practices
Before collecting data, I ensured that my scraping practices were ethical and aligned with best practices:
1. **Checking GOAT’s Terms of Service**: I reviewed GOAT’s website policies to confirm that automated scraping was permissible. Since GOAT does not provide an open API, I limited my requests to avoid server overload.
2. **Respecting Rate Limits**: I included a delay between requests to prevent overwhelming the site.
3. **User-Agent Header**: I set a user-agent in my request headers to mimic a real browser, reducing the risk of being blocked.
4. **Data Usage**: My goal was to analyze publicly available sneaker listings for educational purposes only, without redistributing or monetizing the data.


### How to Get the Data
For students interested in conducting a similar project, here are the key steps:
1. **Identify the Target Website**: Choose a reliable source like GOAT that provides structured sneaker data.
2. **Inspect the Website Structure**: Use browser developer tools (F12 in Chrome) to inspect HTML elements containing product details.
3. **Use Python for Web Scraping**:
   - `requests` to send HTTP requests
   - `BeautifulSoup` to parse HTML and extract relevant information
4. **Extract Relevant Features**: I focused on key attributes such as rank, shoe name, price, release date, product link, and (if available) main color and category.
5. **Store Data in a Pandas DataFrame**: This allows for easy analysis and visualization.
6. **Save Data for Future Use**: Export as a CSV for further exploration.


### Summary of the Dataset
My final dataset includes:
- **182 sneakers**
- **Features:** Rank, shoe name, price, release date, product link, main color (if available), and category (if available)
- **Missing Data:** Some entries lacked information on color and category, which could be filled through further scraping or alternative data sources.


### Interesting Findings (Teaser)
While I will cover detailed Exploratory Data Analysis (EDA) separately, some initial observations include:
- Air Jordan models dominate the top rankings, reflecting their sustained popularity.
- Release dates are clustered around major sneaker release seasons (e.g., January and March).
- Prices vary widely, with some sneakers under $120 and others exceeding $250.


### Further Resources
For those looking to replicate or extend this project, here are some useful resources:
- **Python Libraries**: [requests](https://docs.python-requests.org/en/latest/), [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
- **Web Scraping Guidelines**: [Scrapy Documentation](https://docs.scrapy.org/en/latest/)
- **Sneaker Market Insights**: [GOAT](https://www.goat.com/)


### Access the Code
The full code and dataset are available in my [GitHub repository](#) (replace with actual link).


By following these steps, any Stat 386 student can embark on their own data collection project, gaining valuable skills in web scraping, data processing, and statistical analysis!
