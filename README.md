### Data-Extraction-and-Text-Analysis-using-NLP
## Objective
The primary goal of this project is to automate the extraction of textual data from specified URLs and to perform detailed textual analysis using Natural Language Processing (NLP) techniques. The extracted data is then used to compute various variables aimed at understanding the content’s structure and sentiment.
## Tools and Libraries Used
**Python**: Programming language for script development.
**BeautifulSoup, Selenium, Scrapy**: Libraries used for web scraping to extract content from web pages.
**NLTK, TextBlob**: Libraries used for natural language processing tasks.
**Pandas**: For data manipulation and analysis.
**NumPy**: For numerical operations.

**## Data Extraction and Analysis Details**
## Data Extraction:

Articles are extracted from URLs provided in an Excel file using web scraping tools.
Extracted content includes article titles and main text, avoiding navigation bars, footers, or ads.

**## Textual Analysis:**

Performs sentiment analysis to compute scores like Positive and Negative Scores, Polarity, and Subjectivity.
Calculates readability metrics such as FOG Index, Average Sentence Length, and Percentage of Complex Words.
Detailed word and syllable counts are used to assess text complexity.

**##Output**
The analysis results are structured as per the "Output Data Structure.xlsx", saved in a CSV/Excel format.
Variables include detailed sentiment scores, readability statistics, and text complexity metrics.
