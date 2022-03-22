# Research Exercise 8: Collecting and Modeling the Reprinting and Reuse of Texts (Part 1)


For this week's practicum, you've already begun to read about the conditional probability behind machine learning techniques. We'll be drawing on those methods in the coming weeks as we explore techniques for algorithmically querying a dataset.

The first technique we'll be learning is searching for patterns of text-reuse. In order to do this, we're going to learn how to create a corpus of texts that might be queried 

For **part 1 of this exercise**: you're going to complete the steps outlined below for downloading a data-cleaning (and collecting) software called OpenRefine. Following the steps of a Programming Historian tutorial, you'll use OpenRefine to create two small corpora of text drawing from web URLs and write up a short reflection on what you learn about the the method.

**Part 2 (which we'll complete together in class)** will walk you through the steps for using n-grams patterns of text-re-use.


## Part 1: Collecting documents from the web using OpenRefine

In this exercise, we're going to learn how to step through the processing of web-scraping open-access collections of materials. We're going to use a software called OpenRefine and the web-based URLS of text files and webpages with OCR'd data to fetch and 


### What is Web-Scraping?

**Web-scraping** is a term for computationally collecting data from the internet. "Scrape," "crawl," "spider," and "robot" are all terms used to describe the process of automating the collection of data on the internet. This includes downloading the HTML files of webpages, as well as extracting information from web pages.

### The Ethics of Web-Scraping

In this week's lesson, we'll be fetching and parsing data from **open-access** web resources that allow users to freely use and collect their data. In other cases, the terms and conditions around how you can "scrape" or fetch material from a website are much more murky. We'll be talking more about this in class, but it's absolutely crucial to think about the ethical and legal questions around this method of data collection. Is it legal and ethical to collect data from the internet published by others? What degree of consent do you need from users for research?

A 2019 ruling by the Ninth Circuit court ruled that scraping publicly available databases (The Electronic Frontier Foundation wrote about the ruling in[ an article here](https://www.eff.org/deeplinks/2019/09/victory-ruling-hiq-v-linkedin-protects-scraping-public-data#:~:text=Linkedin%20Protects%20Scraping%20of%20Public%20Data,-Share%20It%20Share&text=In%20a%20long%2Dawaited%20decision,and%20Abuse%20Act%20(CFAA).))

For research involving human participants (this is especially applicable for social media scraping), the general recommendation is to err on the side of caution and request approval from the Institutional Review Board (in this case, Princeton's IRB) for research. 

Just because it may be legal to collect public data on the internet does not mean it is always ethical to do so. There are techniques for anonymizing data (including only excerpts). For a more in-depth study on the question of ethical and legal side of web scraping (and the often murky regulatory mechanism on the subject,) see this article by [this article by Casey Fiesler, Nathan Beard, and Brian C. Keegan](https://cmci.colorado.edu/~cafi5706/ICWSM2020_datascraping.pdf)

###  OpenRefine

![images](../_images/OpenRefine.png)

OpenRefine is a  open-source application for sorting, cleaning data, and building datasets. It has the very handy built-in capacity to interact with  APIs to let us create scripts that let us computationally download data from the web into a spreadsheet. 

OpenRefine is an application that runs in a web browser (like Jupyter notebooks and JupyterLab) *but* it stores all of your data, and data transformations locally––you're only ever interacting with the web when you are calling up a URL to download. We'll be learning more about what OpenRefine can do in class, but for now, follow the instructions below to download the program. 

### 1a. Download OpenRefine

1. Navigate to the OpenRefine [download page](https://openrefine.org/download.html)
2. Follow the instructions to download the OpenRefine (version 3.4.1) kit for your operating system. This will download the app installer for your operating system

- *NOTE*: OpenRefine requires the software Java. If you are on Windows, you will need to download a different version depending on whether or not you have Java. To check whether you have Java, open up PowerShell (your command line interface) and type `java -version`. You will either get an output with the line `java version "your version number"` or nothing. If nothing is returned, this means you don't have Java on your machine.


### 1b. Complete the *Programming Historian* tutorial: Fetching and Parsing Data with OpenRefine

1. Complete the steps for Evan Peter Williamson's ["Fetching and Parsing Data with OpenRefine."](https://programminghistorian.org/en/lessons/fetch-and-parse-data-with-openrefine#cleanup-and-export)
2. The tutorial will take you through two steps for web-scraping with OpenRefine: 
	 -  First, creating a simple dataset of [Shakespeare's 154 sonnets from Project Gutenberg](https://www.gutenberg.org/cache/epub/1105/pg1105.html)
	-  And second, you'll be creating a small corpus of articles from the Library of Congress's [*Chronicling America*](https://chroniclingamerica.loc.gov/)  project, a historical Newspaper database of eighteenth-, nineteenth-, and early-twentieth-century newspapers in the United States. (For more about the project, read here: https://chroniclingamerica.loc.gov/about/)

💡 Tips and Tricks 💡 
-  If you find yourself getting stuck, or want a refresher, you can read another [tutorial I've written on how to download song lyrics from a website like Genius using OpenRefine.](https://github.com/sceckert/IntroDHSpring2021/blob/main/_week6/introduction-to-webscraping-and-open-refine.md)
	-  **NOTE**: Genius allows users to query its database.  Unlike Chronicling America, Genius requires users to sign up for an "API" (an application programming interface) and get a special key in order to programmatically query their database. For instructions on how to do that, see: https://github.com/sceckert/IntroDHSpring2021/blob/main/_week6/preparing-for-webscraping-and-openrefine.md#registering-for-the-genius-api

If you're interested in OpenRefine, see my [quick overview of how OpenRefine can be used to "clean" a dataset](https://github.com/sceckert/IntroDHSpring2021/blob/main/_week6/preparing-for-webscraping-and-openrefine.md#using-openrefine) and this quick overview of [advanced methods for using OpenRefine to fetch material from the web](https://github.com/sceckert/IntroDHSpring2021/blob/main/_week6/advanced-tips-for-webscraping.md#using-openrefine-for-webscraping-advanced-tips)

### 1c. Reflection

Take a minute to jot down some reflections on the two collections of data that you've just created. What kind of information were you able to pass using web-scraping? Are there open-access texts or collections that you would want to fetch using these methods? What considerations might a literary historian who wants to assemble a collection of texts need to keep in mind?

Think back the section of David A. Smith, Ryan Cordell and Elizabeth Maddock Dillon's "Infectious Texts" (2013). How might you use the methods you've learned to collect a corpus of texts that you might use to study the reprinting of short texts (poems, advertisements, news items)? What might a researcher need to take into account?

## Part 2: Algorithmically Identifying Text Reprinting

We'll complete this together in class! For a sneak preview of the method we'll be learning, you can read about the text-matcher algorithm developed for the Middlemarch Critical Histories Project here: [https://github.com/JonathanReeve/text-matcher](https://github.com/JonathanReeve/text-matcher)