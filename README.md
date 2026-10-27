## Description

This workshop evolved from an earlier session on document classification and topic modeling. Through several iterations, we realized that the material assumed a stronger background in text processing with Python than most participants had developed in the previous workshops. Additionally, we were attempting to cover too much, such as reading, cleaning, and preparing data for both document classification and topic modeling, in a single session.

As a result, we decided to split the workshop into two parts, with one dedicated to text data preparation and the other to document classification. This repository contains the code and explanations for working with text data, focusing on datasets from industry archives and data scraped directly from websites.

## Objectives

Through a series of hands-on exercises with Python and a collection of text files, participants will learn to:

* Identify potential data loss resulting from image to text transcription technologies
* Explain when and why a researcher might want to process or prepare a text collection manually for an NLP task
* Evaluate the trade-offs between using a GenAI approach to cleaning text vs a more manual programmatic one 
* Collect data from the web or unstructured files
* Standardize punctuation
* Standardize capitalization
* Removing non-alphanumeric characters
* Tokenize text
* Remove stop words
* Apply a pre-defined vocabulary
* Stem or Lemmatize words, and understand the trade-offs
* Creating a bag-of-words
* Creating a word frequency vector

### Prerequisites

This workshop is intended for participants who have basic programming experience with Python, including loops, conditionals, and lists. No previous experience with JSON is expected. Some familiarity with tree structures and recursion will help, but we will cover these concepts in the context of parsing JSON documents.

### Instructor

Geoffrey Boushey is a computational and research data science specialist at UCSF and a member of the Library's Data Science and Open Scholarship team. Geoff teaches courses and provides consultations on foundational programming, data analysis, and AI techniques including Python, SQL, Unix, and Version Control.

## Data

This workshop uses two main data sources

### Industry Documents Library

The Washington Post Opioid collection provides a prepared dataset from the Industry Archives collection, and provides a good illustration of the way data is preserved and lost through an image-to-text transcription process. 

### Cornell Movie Dataset

This dataset is often used to introduce or test classification and sentiment analysis.

http://www.cs.cornell.edu/people/pabo/movie-review-data/

## Workbooks

### Working-With-Text.ipynb

This workbook reviews how to parse, clean, and edit text data in preparation for common machine learning and natural language processing tasks. 

### Read-All-Files.ipynb

This workbook reviews how to 
* read text from a collection of files into python string variables 
* format the results in a pandas dataframe

### Movie-Review-Web

This workbook reviews how to read and process a movie review directly from the web using the requests module and beautifulsoup, a popular library package used to convert messy formatting (including HTML or other markup tags) into clean text. 

https://pypi.org/project/beautifulsoup4/

## Additional Tools for Web Data Collection

While BeautifulSoup is great for static HTML pages, many modern websites rely on JavaScript to load content or require user interactions (like clicking buttons or filling forms). The tools below are designed to handle these dynamic scenarios, allowing you to collect data from more complex websites.

- **Selenium**: Ideal for collecting data from JavaScript-heavy websites. It allows for browser automation, making it perfect for interacting with dynamic content (e.g., clicking buttons, submitting forms).
  
- **Playwright**: A faster, more efficient alternative to Selenium with multi-browser support (Chrome, Firefox, Safari). Great for collecting data from modern web apps and dynamic content with minimal overhead.

- **Scrapy**: A full-fledged web data collection framework for large-scale projects. It handles things like asynchronous requests, data pipelines, and error management, making it a powerful choice for complex, high-volume tasks.

- 

