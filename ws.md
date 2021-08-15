# Web Scraping

* **Web scraping** : is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.

* Web scraping : is data scraping used for extracting data from websites. Web scraping software may access the World Wide Web directly using the Hypertext Transfer Protocol, or through a web browser. While web scraping can be done manually by a software user, the term typically refers to automated processes implemented using a bot or web crawler. It is a form of copying, in which specific data is gathered and copied from the web, typically into a central local database or spreadsheet, for later retrieval or analysis.

* It is used for contact scraping, and as a component of applications used for web indexing, web mining and data mining, online price change monitoring and price comparison, product review scraping (to watch the competition), gathering real estate listings, weather data monitoring, website change detection, research, tracking online presence and reputation, web mashup and, web data integration.

* Steps :

    * The first thing that we need to do is to figure out where we can locate the links to the files we want to download inside the multiple levels of HTML tags. Simply put, there is a lot of code on a website page and we want to find the relevant pieces of code that contains our data

    * On the website, right click and click on “Inspect”. This allows you to see the raw code behind the site.

    * If you click on this arrow symbol and then click on an area of the site itself, the code for that particular item will be highlighted in the console.

    * start by importing the following libraries.

        * **import requests**
        * **import urllib.request**
        * **import time**
        * **from bs4 import BeautifulSoup**

* Next, we set the url to the website and access the site with our requests library.

    * **url = 'http://web.mta.info/developers/turnstile.html'**
    * **response = requests.get(url)**

* parse the html with BeautifulSoup so that we can work with a nicer, nested BeautifulSoup data structure

    * **soup = BeautifulSoup(response.text, “html.parser”)**

* We use the method .findAll to locate all of our tags.

    * **soup.findAll('a')**

* extract the actual link that we want. Let’s test out the first link.

    * **one_a_tag = soup.findAll(‘a’)[38]**
    * **link = one_a_tag[‘href’]**

* use our urllib.request library to download this file path to our computer. We provide request.urlretrieve with two parameters: file url and the filename

    * **download_url = 'http://web.mta.info/developers/'+ link**
    * **urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:])**

* we should include this line of code so that we can pause our code for a second so that we are not spamming the website with requests. This helps us avoid getting flagged as a spammer.

    * **time.sleep(1)**


