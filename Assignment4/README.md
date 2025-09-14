# Assignment 4: Web Scraping Projects

## Objective
The goal of this assignment is to practice web scraping techniques using Python. You will extract structured data from different live websites, parse it, and store the results in a clean tabular format for analysis.

---

## Tasks

### Q1: Scrape Books from Books to Scrape
Website: [Books to Scrape](https://books.toscrape.com/)

Steps:
1. Scrape all book details across all pages.  
2. Extract:  
   - Title  
   - Price  
   - Availability (In stock / Out of stock)  
   - Star Rating (One to Five)  
3. Store results in a Pandas DataFrame.  
4. Export results to `books.csv`.  

Libraries: `requests`, `BeautifulSoup`, `pandas`  

---

### Q2: Scrape IMDB Top 250 Movies
Website: [IMDB Top 250](https://www.imdb.com/chart/top/)  

Steps:
1. Scrape top 250 movies.  
2. Extract:  
   - Rank (1–250)  
   - Movie Title  
   - Year of Release  
   - IMDB Rating  
3. Store results in a Pandas DataFrame.  
4. Export results to `imdb_top250.csv`.  

Libraries: `selenium` or `playwright`, `pandas`  

---

### Q3: Scrape World Cities Weather
Website: [Time and Date Weather](https://www.timeanddate.com/weather/)  

Steps:
1. Scrape weather details of top world cities.  
2. Extract:  
   - City Name  
   - Temperature  
   - Weather Condition (Clear, Cloudy, Rainy, etc.)  
3. Store results in a Pandas DataFrame.  
4. Export results to `weather.csv`.  

Libraries: `requests`, `BeautifulSoup`, `pandas`  

---



