# PriceStats-Assessment

Once downloaded files in terminal go into the folder with the files

## Download dependencies
Run: pip install -r requirements.txt

## Run Script
Run: python ProdScraper.py

## How the code works

1. sqlConnect(db_path)
Gets the uniform resource identifier(URI) of the database file. Then using the sqlite3 function connect() to connect to the database. If this is not happening it returns an error and closes the script
2. create_table(connection, SQL_Table)
Creates a cursor, deletes all the table if it exists, then using a SQLite format to create a new SQLite database
3. findPageNumber(URL)
Using the requests python library, to get the information in text format. Then using BeautifulSoup python library to parse the HTML data. Using BeatifulSoup to find the number of pages. Get the total number of pages then returns that to be used to loop through the scrapeProducts function for all the pages
4. scrapeProducts(pages)

5. 
