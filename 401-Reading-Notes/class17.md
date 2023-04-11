# 401 Class 17 Reading Notes

## Summary: This class is about Web Scraping

**Prompt**: Write a statement addressing why web scraping matters.

Web scraping is a critical skill for studying and analyzing data in this module because it allows us to collect and analyze large amounts of data from various sources on the internet. In this module, we are studying data analysis and machine learning techniques that require large datasets for training and testing. 

Web scraping enables us to collect and preprocess data from various websites and online sources, making it easier to create high-quality datasets for our analysis. Additionally, web scraping allows us to access and analyze data that may not be readily available through traditional data sources, such as social media, news articles, and customer reviews. Therefore, web scraping is an essential tool that enables us to collect and analyze data effectively and efficiently, ultimately improving the accuracy and effectiveness of our analysis and machine learning models.

**Q:** What are the key differences between scraping static and dynamic websites?

**A** :Static websites are composed of HTML pages that are served to the client's browser exactly as they were stored on the server. In contrast, dynamic websites are generated on the server-side, often with the use of programming languages such as PHP, Python, or Ruby. The key differences between scraping static and dynamic websites are as follows:

HTML structure: Static websites have a fixed structure that is easily identifiable and can be scraped using basic web scraping techniques such as parsing HTML tags. Dynamic websites, on the other hand, have a more complex structure that requires additional techniques such as web automation or APIs to access the data.

Data availability: In a static website, all the data is present on the page and can be easily scraped. In contrast, dynamic websites may require additional requests to the server to load more data, which makes scraping more challenging.

Data refresh: Dynamic websites often refresh data frequently, and the new data replaces the old data on the page. As a result, web scrapers may need to wait for the data to refresh before scraping the new data. In contrast, static websites retain the same data until the page is manually updated.

User interaction: Dynamic websites often rely on user interaction to load new data, such as clicking on buttons or filling out forms. Web scrapers may need to simulate user interaction through web automation to scrape this data, which can be more challenging than scraping static websites.

In summary, static websites are relatively easy to scrape because of their simple HTML structure and static data. Dynamic websites, on the other hand, may require more advanced techniques such as web automation or APIs to access the data, but can provide more up-to-date and dynamic data.

**Q**: Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.

**A**: Web scraping is a powerful tool for data extraction, but it can be risky if done improperly. To avoid getting blocked while scraping websites, here are three techniques or best practices you can employ:

- Respect robots.txt: Robots.txt is a file used by websites to communicate with web crawlers about which parts of the site can be crawled and which cannot. It is essential to respect this file and follow the guidelines set out in it. Failing to do so may result in your IP address being blocked or your scraping attempts being detected as malicious activity. You can check for the robots.txt file on a website by adding /robots.txt to the end of its URL.

- Use scraping libraries or tools: There are many scraping libraries and tools available that are designed to help you scrape websites without getting blocked. These tools often come with features that enable you to limit the number of requests per second, rotate user agents and IP addresses, and add delays between requests. Some popular scraping libraries include BeautifulSoup, Scrapy, and Selenium.

- Mimic human behavior: To avoid detection, it is essential to make your scraping activities look as human-like as possible. This includes setting realistic user agents, limiting the number of requests per second, adding delays between requests, and avoiding scraping at unusual times or patterns. You can also mimic human behavior by clicking on links and buttons, filling out forms, and scrolling through pages as a human would.

- In summary, to avoid getting blocked while scraping websites, you should respect robots.txt, use scraping libraries or tools, and mimic human behavior as much as possible. By following these techniques and best practices, you can increase your chances of scraping websites successfully while avoiding detection.

**Q**: What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.

**A**:Playwright is an open-source Node.js library for automating web browsers, which was created by Microsoft. Playwright is designed to make it easy to write reliable, fast, and stable browser automation scripts for tasks such as testing, web scraping, and web application development. Playwright supports multiple browsers, including Chromium, Firefox, and WebKit, and provides a simple API for interacting with web pages, including clicking on links and buttons, filling out forms, and scraping data.

Playwright assists in web scraping tasks by providing a high-level API that allows you to interact with web pages as a user would. This means that you can write scripts that perform complex interactions, such as scrolling through pages, clicking on links, and filling out forms, without having to write low-level code for each interaction. Additionally, Playwright's support for multiple browsers allows you to scrape data from different websites that may have different rendering engines or JavaScript behavior.

One use case where Playwright would be particularly beneficial is in scraping data from websites that use a lot of JavaScript. Since Playwright can interact with JavaScript just like a user would, it can easily scrape data from websites that generate content dynamically using JavaScript. For example, suppose you want to scrape data from an e-commerce website that loads product information dynamically as the user scrolls down the page. In that case, you can use Playwright to simulate the user scrolling down the page and scraping the data as it loads.

Another use case where Playwright would be beneficial is in scraping data from websites that require login credentials. Playwright provides a simple API for filling out login forms and interacting with authenticated pages, which makes it easy to scrape data from websites that require authentication.

In summary, Playwright is a powerful tool for web scraping tasks, as it provides a high-level API for interacting with web pages and supports multiple browsers. Playwright's support for JavaScript and its ability to interact with login forms and authenticated pages make it particularly beneficial for scraping data from dynamic websites and websites that require authentication.

**Q**: Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.

**A**: XPath is a query language used to navigate and select elements from an XML or HTML document. In web scraping, XPath is commonly used to extract data from HTML documents by selecting specific elements, attributes, or text content.

An XPath expression is a path to an element in an HTML document that consists of a series of nodes separated by slashes. Each node represents an element, attribute, or text content in the document.

XPath expressions can be used in many programming languages and tools for web scraping, including Python's lxml and BeautifulSoup libraries and browser automation tools such as Selenium and Playwright. By using XPath expressions to select specific elements from HTML documents, web scrapers can extract structured data from web pages more easily and efficiently.


## Sources: 

ChatGPT

https://scrapingant.com/blog/scrape-dynamic-website-with-python

https://en.wikipedia.org/wiki/Web_scraping

https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/

https://www.youtube.com/watch?v=H2-5ecFwHHQ&t=60s

https://www.youtube.com/watch?v=yp1o9biMMWU

https://www.crummy.com/software/BeautifulSoup/

 ## Things I want to know more about

Web Scraping Tools and how its used for training data 
