# WebScraping:Website-Pricebaba-
We have scraped the website Pricebaba. We have created a program that takes price range value as input and returns price and VFM score of mobile phones in that range.

The code you have provided is a Python program that crawls the Pricebaba website to get the price and VFM score of mobile phones in a given price range.

The first function, get_model_price(), takes a URL as input and returns the price and VFM score of the mobile phones listed on that page. It does this by using the BeautifulSoup library to parse the HTML of the page and extract the relevant information.

The second function, get_pages(), takes a URL as input and recursively crawls all the pages of the website starting from that page. It uses the re library to extract the page number from the URL.

The main function first asks the user to enter the lower and upper limits of the price range. It then calls the get_pages() function to crawl the website and get the price and VFM score of all the mobile phones in the given price range. Finally, it creates a Pandas DataFrame to store the results and prints the DataFrame.

Here is a more detailed explanation of the code:

The get_model_price() function first imports the requests and BeautifulSoup libraries. It then defines a few regular expressions to extract the relevant information from the HTML. The function then makes a request to the URL and parses the response using BeautifulSoup. Finally, it extracts the price and VFM score of the mobile phones and returns them as a tuple.
The get_pages() function also imports the requests and BeautifulSoup libraries. It then defines a regular expression to extract the page number from the URL. The function then makes a request to the URL and parses the response using BeautifulSoup. Finally, it extracts the page number and calls itself recursively to crawl the next page.
The main function first defines a dictionary to store the page URLs. It then asks the user to enter the lower and upper limits of the price range. The function then calls the get_pages() function to crawl the website and get the price and VFM score of all the mobile phones in the given price range. Finally, it creates a Pandas DataFrame to store the results and prints the DataFrame.
I hope this explanation is helpful. Please let me know if you have any other questions.
