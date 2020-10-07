
<img src="https://scontent.fslv1-2.fna.fbcdn.net/v/t1.0-9/120830800_795875101206008_6566579393005725982_n.jpg?_nc_cat=111&_nc_sid=730e14&_nc_ohc=96NGCctGOWsAX9sps1_&_nc_ht=scontent.fslv1-2.fna&oh=b7ab157cc52372f811c8fe12784e0d17&oe=5FA4B644" alt="sturtured data" width="1000" height="250">

# Content
---   
*  [What is Web scraping?]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#what-is-web-scraping)                
*  [The basics of web scraping]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#the-basics-of-web-scraping)  
*  [Can you scrape from all the websites?]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#can-you-scrape-from-all-the-websites) 
*  [Techniques of Web Scraping]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#techniques-of-web-scraping) 
*  [How do we do web scraping?]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#how-do-we-do-web-scraping)
*  [Uses of Web Scraping]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#uses-of-web-scraping)                                                     
*  [Different tools and library for web scraping]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#different-tools-and-library-for-web-scraping)
*  [Challenges to Web Scraping]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#challenges-to-web-scraping)
*  [Future of  Web Scraping]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#future-of-web-scraping)
*  [Bibliography]( https://github.com/yusufsheikh531/_Web_Scraping_/blob/worked/README.md#bibliography) 


# What is Web scraping?
---
*Web scraping refers to the extraction of data from a website. This information is collected and then exported into a  format that is more useful for the user such as .csv file or spreadsheet.* <img align="right" src="https://www.edureka.co/blog/wp-content/uploads/2018/11/Untitled-1.jpg" alt="sturtured data" width="500" height="150">
*	poorly structured data from websites --> into a structured format eg. spreedsheet      
*	 help you track changes to data online.
*	There are many languages used for web scraping example node.js, c, c++, php etc.<br>
    But Python is the best language because it is the easiest language to learn because of its syntax.
   
   
# The basics of web scraping
---
It have 2  parts-The crawler (like a horse) ,The scraper (like a charoit)<br>
The crawler leads the scraper, as if by the hand, through the internet, where it extracts the data requested.
<img align="right" src="https://www.scrapinghub.com/wp-content/uploads/2019/05/crawler.png" alt="sturtured data" width="200" height="150">	
   ### The crawler 
   Also called “spider”                                                                                                                           
   is an artificial intelligence that browses the internet to index and search for content by following links and exploring.
   
   ### The scraper<img align="right" src="https://www.scrapinghub.com/wp-content/uploads/2019/05/scraper.png" alt="sturtured data" width="200" height="100">
   A web scraper is a specialized tool designed to accurately and quickly extract data from a web page.



# Can you scrape from all the websites?
---
Scraping makes the website traffic to spike and may cause breakdown of the website server. Thus, not all of the websites allow people to scrape.
How do you know which websites are allowed or not?
just simply put robots.txt after the url that you want to scrape.<br>

Take Google.com for an example:

<!--'![robots.txt](https://miro.medium.com/max/700/1*pe7HHTIwhbqJJcEfsYcfaA.png)'-->
<img src="https://miro.medium.com/max/700/1*pe7HHTIwhbqJJcEfsYcfaA.png" alt="robots.txt" width="700" height="500">
 
You can see that<br>
*	Google does not allow web scraping for many of its sub-websites. However, it allows certain path like ‘/m/finance’ and thus if you want to collect information on finance then this is a completely legal place to scrape.
*	On first row Google specifies the rules for all of the user-agents but website may give certain user-agent special permission so you may want to refer to information there.


# Techniques of Web Scraping:
---
 There are two ways of extracting data from websites, the Manual extraction technique, and the automated extraction technique.<br>
`1. Manual Extraction Techniques:`  Manually copy-pasting the site content comes under this technique. Though tedious, time taking and repetitive it is an effective way to scrap data from the sites having good anti-scraping measures like bot detection.

` 2. Extraction Techniques:`  web scraping software is used to automatically extract data from sites based on user requirement.

* **HTML Parsing:** Parsing means to make something understandable to be analyzing it part by part. To wit, it means to convert the information in one form to another form that is     easy to that is easier to work on with. HTML parsing means taking in the code and extracting relevant information from it based on the user requirement. Mainly executed using   JavaScript, the target as the name suggests are HTML pages.

* **DOM Parsing:** The Document Object Model is the official recommendation of the World Wide Web Consortium. It defines an interface that enables a user to modify and update the     style, structure, and content of the XML document.

* **Web Scraping Software:**  Nowadays, many web scraping tools are available or are custom build on users need to extract required desiring information from millions of websites.

# How do we do web scraping?
---
There are 2 different approaches for web scraping depending on how does website structure their contents.<br> 

>**Approach 1:** *If website stores all their information on the HTML front end, you can directly use code to download the HTML contents and extract out useful information.*<br>

    Steps:
    1.  Inspect the website HTML that you want to crawl.
    2.	Access url of the website using code and download all the HTML contents on the page.
    3.	Format the downloaded content into readable format.
    4.	Extract out useful information and save into a structured format.
    5.	For information displayed on multiple pages of website, you may need to repeat step 2–4 to have the complete information.

 **Pros and Cons for this approach:** It is simple and direct. However, if website front end structure changes then you need to adjust your code accordingly.<br>
 
 >**Approach 2:** *If website stores data in API and the website queries the API each time when user visit the website, you can simulate the request and directly query data from >the API.*<br>

    Steps:
    1.	Inspect 'XHR' network section of the URL that you want to crawl.
    2.	Find out the request response that gives you the data that you want.
    3.	Depending on the type of request(post or get) and also the request header & payload, simulate the request in your code and retrieve the data from API. Usually the data got from API is in pretty neat format.
    4.	Extract out useful information that you need.
    5.	For API with limit on query size, you will need to use ‘for loop’ to repeatedly retrieve all the data.

 **Pros and Cons for this approach:** It is definitely a preferred approach if you can find the API request. The data you receive will be more structured and stable. This is    because compared to website front end, it is less likely for the company to change its backend API. However, it is a bit more complicated than the first approach especially if  authentication or token is required.


# Different tools and library for web scraping
---
<ins> **Tool for Web Scraping:** </ins> 

Web Scraping tools are specifically developed for extracting data from the internet. Some of the most popular Web Scraping tools are:
*	[Import.io](https://www.import.io/)
*	[Webhose.io](https://webhose.io/)
*	[Dexi.io](https://www.dexi.io/)
*	[Scrapinghub](https://www.scrapinghub.com/)
*	[Parsehub](https://www.parsehub.com/)

<ins>**The most commonly used library for web scraping in Python are :**</ins><br>

 **`Beautiful Soup:`** It helps you parse the HTML or XML documents into the readable format. It allows you to search different elements within the documents and help you retrieve required information faster.<br>
**`Requests:`** It is a Python module which you can send HTTP requests to retrieve contents. It helps you to access website HTML contents or API by sending Get or Post requests.<br>
**`Selenium:`** It is widely used for website testing and it allows you to automate different events(clicking, scrolling etc) on the website to get the results you want.
You can either use Requests + Beautiful Soup or Selenium to do web scraping. Selenium is preferred if you need to interact with website(JavaScript events) and if not I will prefer Requests + Beautiful Soup because its faster and easier.<br>


# Uses of Web Scraping
---
  ### Price Monitoring
Revolutionize day-to-day business with web scraped product data and dramatically increase your company’s competitiveness. From automatic pricing solutions to profitable investment insights, this data moves mountains.
<!--⛔️ magic start -->
<details>
<summary>EXAMPLES (click HERE to expand)</summary>
	
*	Dynamic Pricing and Revenue Optimization
*	Competitor Monitoring
*	Product Trend Monitoring
*	Investment Decision Making
*	Brand and MAP Compliance
        </details>
<!-- ⛔️ MD-MAGIC-EXAMPLE:END -->

  ### Alternative Data For Finance
Unearth alpha and radically create value with web data tailored specifically for investors. The decision-making process has never been as informed, nor data as insightful – and the world’s leading firms are increasingly consuming web scraped data, given its incredible strategic value.
<!--⛔️ magic start -->
<details>
<summary>EXAMPLES (click HERE to expand)</summary>
	
*	Extracting Insights from SEC Filings
*	Estimating Company Fundamentals
*	Public Sentiment Integrations
*	News Monitoring
</details>
<!-- ⛔️ MD-MAGIC-EXAMPLE:END -->

  ### Market Research
Market research is critical – and should be driven by the most accurate information available. High quality, high volume, and highly insightful, web scraped data of every shape and size is fueling market analysis and business intelligence across the globe.
<!--⛔️ magic start -->
<details>
<summary>EXAMPLES (click HERE to expand)</summary>
	
*	Market Trend Analysis
*	Market Pricing
*	Optimizing Point of Entry
*	Research & Development
*	Competitor Monitoring
</details>
<!-- ⛔️ MD-MAGIC-EXAMPLE:END -->

  ### Real Estate
The digital transformation of real estate in the past twenty years threatens to disrupt traditional firms and create powerful new players in the industry. By incorporating web scraped product data into everyday business, agents and brokerages can protect against top-down online competition and make informed decisions within the market.
<!--⛔️ magic start -->
<details>
<summary>EXAMPLES (click HERE to expand)</summary>
	
*	Appraising Property Value
*	Monitoring Vacancy Rates
*	Estimating Rental Yields
*	Understanding Market Direction
</details>
<!-- ⛔️ MD-MAGIC-EXAMPLE:END -->

  ### Sentiment Analysis
For businesses that want to understand what their clientele – and competition – truly think and feel, web scraped product data and sentiment analysis are a match made in heaven. Guess no more and eradicate bias from your interpretations by incorporating and integrating bewildering amounts of relevant, insightful data from your industry.
<!--⛔️ magic start -->
<details>
<summary>EXAMPLES (click HERE to expand)</summary>
	
*	Investment Decision Making
*	Product Monitoring
*	Brand and Company Monitoring
*	Product Development
*	Politics and Campaigns
 </details>
<!-- ⛔️ MD-MAGIC-EXAMPLE:END -->

  ### News & Content Monitoring
Modern media can create outstanding value or an existential threat to your business - in a single news cycle. If you’re a company that depends on timely news analyses, or a company that frequently appears in the news, web scraping is the ultimate solution for monitoring, aggregating and parsing the most critical stories from your industry.
<!--⛔️ magic start -->
<details>
<summary>EXAMPLES (click HERE to expand)</summary>
	
*	Investment Decision Making
*	Online Public Sentiment Analysis
*	Competitor Monitoring
*	Political Campaigns
</details>
<!-- ⛔️ MD-MAGIC-EXAMPLE:END -->


# Challenges to Web Scraping:
---
*	`Data Warehousing:`  If the data warehousing infrastructure is not properly built then the searching, storing and exporting of this data will become a cumbersome task. Hence, for large-scale data extraction, there needs to be a perfect data warehousing system without any flaws and faults.

*	`Website Structure Changes:` Every website periodically updates its user interface to improve its attractiveness and experience. This requires various structural changes too. Since the web scrapers are set up according to the code elements of the website at that time, they require changes too. So, they require changes weekly too to target the correct website for data scraping as incomplete information regarding the website structure will lead to improper scraping of data.

*	`Anti-Scraping Technologies:` Some websites use anti-scraping technologies that thwart away any scraping attempt. They apply a dynamic coding algorithm to prevent any bot intervention and use the IP blocking mechanism. It requires a lot of time and money to work around such anti-scraping technologies.

*	`Quality of Data Extracted:` Records that do not meet the quality of information required will affect the overall integrity of the data. Making sure that the Data Scraped meets the quality guidelines is a difficult task as it needs to be done in real-time.


# Future of Web Scraping:
---
 As there are some challenges and opportunities for data scraping. Since we are on the verge of webtransformation, data-scraping in combination with big data can provide the company’s market intelligence and help them identify critical trends and patterns and identify the best opportunities and solutions. Hence, it won’t be wrong to say that Webscraping can be upgraded to the better soon.




# Bibliography
---
*	www.scrapinghub.com
*	www.parsehub.com
*	www.geeksforgeeks.org
*	www.wikipedia.org

