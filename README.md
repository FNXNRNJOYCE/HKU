This is the guidebook of our repository.
This repository contains all the source codes of Group 13, including data crawling, data cleaning, and analytical codes such as word frequency analysis and sentiment analysis. 

The first stage involves running two crawler scripts that collect 500 news articles each from Fox News and The Guardian. 
Executing the Fox News crawler produces an intermediate file named foxnews_articles.xlsx as well as the final crawled dataset foxnews_articles_crawled.xlsx. 
The Guardian crawler, which retrieves articles through the official Content API using the keyword abortion, generates the file guardian_abortion_articles_us.csv. 
These files together constitute the raw corpus used for all subsequent steps.

After collecting the raw datasets, the next stage uses the cleaning script located in the analysis folder, primarily the word_frequency file.
Although designed for word frequency preparation, this script also includes data cleaning preprocess.
The cleaning process produces four standardized datasets, fox_clean_sentiment_analysis.csv and fox_clean_word_frequency.csv for Fox News, and guardian_clean_sentiment_analysis.csv and guardian_clean_word_frequency.csv for The Guardian. 
These cleaned files ensure consistent formatting and are the inputs for every later analysis task.

Based on the cleaned datasets, the analysis scripts in the analysis directory are used to complete various forms of textual analysis, including word frequency visualization and sentiment scoring. 
Each script reads the appropriate cleaned dataset and outputs figures or statistical results that support the final research findings. 

This structured workflow ensures that every stage, from crawling to cleaning to analysis, is reproducible.
