# Web Scraping
Using BeautifulSoup

The purpose of each code is to scrape news articles from the BBC website in different languages, specifically Igbo, Yoruba, Hausa, and Pidgin. the following steps were accomplshed:

Firstly, the necessary packages are installed, BeautifulSoup and Requests, using the pip package manager.

The below codes scrape news headlines and articles from four websites of (https://www.bbc.com) and organize the extracted data into a pandas dataframe.

The text from each headline and article is extracted using the BeautifulSoup library and stored as tuples in a list. The list is then used to create a pandas dataframe.

The headline and body of each article are combined into a single text and stored in a new column in the dataframe called 'Text'.

The original 'Headline' and 'Body' columns are dropped and a new column called 'Language' is added to the dataframe, with the value as either igbo, yoruba, hausa, or pidgin, for every row.

The four dataframes are concatenated into the four major languages in Nigeria and the rows are shuffled.

The shuffled data frame is split in the ratio of 70 to 30 for train and test data, after which the test label is dropped from the test data. Both train and test data are saved as csv files which are kept in the 'nigerian_4lang.zip' folder.

