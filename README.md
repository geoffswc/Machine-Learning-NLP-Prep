# Machine-Learning-NLP-Prep

python review prior to machine learning and natural language processing workshop

## Overview

This repository contains workbooks and links used during the "python background and preparation" workshop held at the UCSF Library on Dec 3, 2019. 

This workshop was designed to provide a review of python programming skills and techniques that will be used extensively in the machine learning and natural language processing workshops on Dec 10 and Dec 17. This workshop also provides a greater focus on file I/O and string/text manipulation in preparation for document classification in the NLP workshop.

## Data

This workshop uses data from the Cornell Movie Review dataset http://www.cs.cornell.edu/people/pabo/movie-review-data/

This workshop will use the polarity dataset v1.1 http://www.cs.cornell.edu/people/pabo/movie-review-data/mix20_rand700_tokens_0211.tar.gz

To run the workbooks below, download and unzip the polarity dataset, and move the "mix20_rand700_tokens_0211" folder into the directory containing the two jupyter notebooks.

### Working-With-Text.ipynb

This workbook reviews how to parse, clean, and edit text data in preparation for common machine learning and natural language processing tasks. 

### Read-All-Files.ipynb

This workbook reviews how to 
* read text from a collection of files into python string variables 
* format the results in a pandas dataframe

### Movie-Review-Web

This workbook reviews how to read and process a movie review directly from the web using the requests module and beautifulsoup, a popular library package used to convert messy formatting (including HTML or other markup tags) into clean text. 

https://pypi.org/project/beautifulsoup4/

### Additional Tools for Web Data Collection

While BeautifulSoup is great for static HTML pages, many modern websites rely on JavaScript to load content or require user interactions (like clicking buttons or filling forms). The tools below are designed to handle these dynamic scenarios, allowing you to collect data from more complex websites.

- **Selenium**: Ideal for collecting data from JavaScript-heavy websites. It allows for browser automation, making it perfect for interacting with dynamic content (e.g., clicking buttons, submitting forms).
  
- **Playwright**: A faster, more efficient alternative to Selenium with multi-browser support (Chrome, Firefox, Safari). Great for collecting data from modern web apps and dynamic content with minimal overhead.

- **Scrapy**: A full-fledged web data collection framework for large-scale projects. It handles things like asynchronous requests, data pipelines, and error management, making it a powerful choice for complex, high-volume tasks.

