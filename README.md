## Description

This repository contains materials for a hands-on workshop on preparing text data for natural language processing (NLP) and machine learning with Python. Using text from web pages, document collections, and prepared datasets, participants learn how to collect, inspect, clean, standardize, and transform text into formats suitable for computational analysis.

The workshop introduces common text-processing tasks such as tokenization, punctuation and capitalization normalization, stop-word removal, stemming and lemmatization, vocabulary filtering, and the creation of bag-of-words and word-frequency representations. It also examines how text can be lost or altered during processes such as image-to-text transcription and encourages participants to consider the trade-offs between manual, programmatic, and generative AI approaches to preparing text data.

These materials grew out of an earlier workshop covering document classification and topic modeling. That workshop attempted to introduce text preparation and downstream NLP methods in a single session. Because preparing text is both a substantial technical task and an important part of the research process, the material was separated into two workshops. This repository focuses on text collection and preparation, providing the foundation for subsequent work in document classification and other NLP methods.

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

### E-Cig-Marketing.ipynb

Generate a wordcloud using topics drawn from an industry documents tobacco collection prepared dataset. 

### Movie-Review-Web

This workbook reviews how to read and process a movie review directly from the web using the requests module and beautifulsoup, a popular library package used to convert messy formatting (including HTML or other markup tags) into clean text. 

https://pypi.org/project/beautifulsoup4/

### Working-With-Text.ipynb

This workbook reviews how to parse, clean, and edit text data in preparation for common machine learning and natural language processing tasks. 

### Read-All-Files.ipynb

This workbook reviews how to 
* read text from a collection of files into python string variables 
* format the results in a pandas dataframe

### Washington-Post-Data.ipynb

Read and prepare a dataset containing opioids articles and documents from the Washington Post 

## Additional Tools for Web Data Collection

While BeautifulSoup is great for static HTML pages, many modern websites rely on JavaScript to load content or require user interactions (like clicking buttons or filling forms). The tools below are designed to handle these dynamic scenarios, allowing you to collect data from more complex websites.

- **Selenium**: Ideal for collecting data from JavaScript-heavy websites. It allows for browser automation, making it perfect for interacting with dynamic content (e.g., clicking buttons, submitting forms).
  
- **Playwright**: A faster, more efficient alternative to Selenium with multi-browser support (Chrome, Firefox, Safari). Great for collecting data from modern web apps and dynamic content with minimal overhead.

- **Scrapy**: A full-fledged web data collection framework for large-scale projects. It handles things like asynchronous requests, data pipelines, and error management, making it a powerful choice for complex, high-volume tasks.

- 

