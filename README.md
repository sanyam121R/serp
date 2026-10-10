# SERP - Search Engine Results Page

Building a search engine like Google, Brave, Bing, etc.
Practical Advanced Learning for:
- Node.js
- NestJS
- MongoDB
- Redis BullMQ
- Meilisearch
- Web Crawling
- Next.js
- Advanced Data Structures
- Advanced Algorithms

## Crawling & Scraping Concepts

* **URL Discovery & Frontiers**: How a crawler manages a queue of URLs to visit next (Breadth-First Search vs. Depth-First Search).
* **Deduplication**: Using hash sets or Bloom filters to avoid visiting the same URL multiple times.
* **Politeness & Rules**: Parsing and respecting robots.txt files and setting rate limits or download delays so you do not overload target servers.
* **Handling JavaScript & Headless Browsers**: Managing dynamic sites using tools like Playwright or Puppeteer when plain HTTP requests return empty content.
* **Anti-Bot Bypassing**: Managing IP rotation, rate limiting, and user-agent headers safely and ethically.


### Steps system must follow
- I need to create a web crawler to discover the data on the Internet
- Then index them and store in special database that maps keywords to the urls they appear on.
- APIs which will provide the response to the queries

### Web Crawler
How does web crawler works - The Chain Reaction
- **The seed** - we give the crawler a list of a few starting websites 
- **Download** - The crawler visits the page and downloads the HTML text.
- **Extract** - extracts the meta data 
    - **The content** - the text, titles, descriptions -> save to the database
    - **The links** - every url pointing to the other websites
- **Repeat** - Adds those new URLs to a “to-do list” (called a crawl frontier) and visit them next