# Web Crawler

## How does web crawler works - The Chain Reaction

- **The seed** - we give the crawler a list of a few starting websites 
- **Download** - The crawler visits the page and downloads the HTML text.
- **Extract** - extracts the meta data 
    - **The content** - the text, titles, descriptions -> save to the database
    - **The links** - every url pointing to the other websites
- **Repeat** - Adds those new URLs to a “to-do list” (called a crawl frontier) and visit them next