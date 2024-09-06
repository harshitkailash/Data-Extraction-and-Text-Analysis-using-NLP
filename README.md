## Data-Extraction-and-Text-Analysis-using-NLP
## Objective
The primary goal of this project is to automate the extraction of textual data from specified URLs and to perform detailed textual analysis using Natural Language Processing (NLP) techniques. The extracted data is then used to compute various variables aimed at understanding the content’s structure and sentiment.
## Tools and Libraries Used
**Python**: Programming language for script development.
**BeautifulSoup, Selenium, Scrapy**: Libraries used for web scraping to extract content from web pages.
**NLTK, TextBlob**: Libraries used for natural language processing tasks.
**Pandas**: For data manipulation and analysis.
**NumPy**: For numerical operations.

## **Data Extraction and Analysis Details**
## Data Extraction:

Articles are extracted from URLs provided in an Excel file using web scraping tools.
Extracted content includes article titles and main text, avoiding navigation bars, footers, or ads.

## Textual Analysis:

Performs sentiment analysis to compute scores like Positive and Negative Scores, Polarity, and Subjectivity.
Calculates readability metrics such as FOG Index, Average Sentence Length, and Percentage of Complex Words.
Detailed word and syllable counts are used to assess text complexity.

## Output
The analysis results are structured as per the "Output Data Structure.xlsx", saved in a CSV/Excel format.
Variables include detailed sentiment scores, readability statistics, and text complexity metrics.

# Code Explanation for Data Extraction and NLP Analysis Project

## Data Extraction:

** 1. Import Libraries:**

pandas for data manipulation.
goose3 for extracting content from web pages.
os for handling file and directory operations.

** 2. Read Input Data:**

Loading URLs from an Excel file into a pandas DataFrame.

**3. Setup Output Directory**:

Creating a directory where extracted articles will be stored

**4.Article Extraction Loop**:

Iterating through each row in the DataFrame to extracting the article using the URL provided.
Using Goose to fetch the article's title and main text.
Saving the article to a text file named with its URL_ID.

## Text Analysis:

**1. Import NLP Libraries**:

TextBlob for basic NLP tasks like sentiment analysis.
nltk for more complex NLP tasks such as tokenization and frequency analysis.
syllapy for counting syllables in words.

**2. Download NLTK Resources**:

Downloading necessary datasets for tokenization and stopwords removal.

**3. Define Text Analysis Function**:

The function processes the text to extract various metrics such as word count, sentence count, average word length, syllables per word, complex word count, FOG Index, and sentiment scores.

**4. Perform Analysis on Extracted Articles**:

Looping through all text files in the output directory, read the article text, and use the analyze_text function to compute the analysis variables.

**5. Save Analysis Results**:

Compiling results into a DataFrame, reorder the columns as specified in the output structure, and save the DataFrame to an Excel file.
