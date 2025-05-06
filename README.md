# Web-Scraper-for-Books-MongoDB-and-Python
## Personal Project for Web Scraping using MongoDB and Python (Scrapy module)

### Explanation
In this project, we have implemented a web scraper for books on the Internet. Specifically, this project targets books on the website https://books.toscrape.com/. Below is the example of how the books are presented on the website.

<img width="800" alt="image" src="https://github.com/user-attachments/assets/ba613474-d41a-4b62-991d-d3c575a42ab2" />
<p></p>

In order to scrape all needed data (`title`, `URL` and `price` in this project), we use Python with Scrapy module to access HTML and CSS code of the website and get the needed data. Following that, since one page only contains up to 20 books, we apply the web crawler to recursively iterate through Next page button URL and scrape all books. Finally, we connect MongoDB and our crawler using `pymongo` to store everything in the database. The code is then adapted to check for repetition in case of multiple runs using the scraper. This is done by checking for any matches in hashes of URLs of stored books. The `SHA256` algorithm is applied for hashing. 

### Result

Every separate item is stored in JSON format and stored in `books_collections.json` file in this directory. Example: 


<img width="800" alt="image" src="https://github.com/user-attachments/assets/c5f3e1e7-496a-4fb9-9d6b-9c772d121c4b" />

### Conclusion

We have successfully implemented Web Scraper for Book collections using MongoDB and Python.
<p> </p>
<p></p>
<br>

Batyrkhan M 2025
