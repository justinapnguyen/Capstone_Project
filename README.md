Would you buy their drugs?
----------------------------

We are interested in performing some NLP and sentiment analysis on reviews for weight loss treatment drugs. We want to analyze public sentiment surrounding Ozempic, a semaglutide drug initially developed for type 2 diabetes but also used off-label for weight loss. Our analysis provides valuable insights into public opinions and attitudes towards the drug, helping healthcare professionals and stakeholders make informed decisions.

There are currently six FDA-approved weight loss drugs on the market. We will be looking at five of them because the last drug, **setmelanotide (Imcivree)** is specifically approved for people with a certain rare genetic disorder. The drugs used for comparison are bupropion-naltrexone (Contrave), liraglutide (Saxenda), orlistat (Xenical, Alli), phentermine-topiramate (Qsymia), and semaglutide (Wegovy).

Table of Contents
-----------------

1. Web Scraping
2. Preprocessing Data
3. Exploratory Data Analysis (EDA)
4. Natural Language Processing (NLP)
5. Logistic Regression (Unigrams)
6. Logistic Regression (Bigrams)
7. Logistic Regression (Trigrams)


---------------
1. Web Scraping

Using a technique called Beautiful Soup to scrap the data from Drugs.com to get the necessary information for this Capstone project. We are retrieving the reviews and the information associated with it.

OUTPUT: clean_raw_drug_reviews.csv (This dataset has 5,233 rows and 9 columns.)

---------------------
2. Preprocessing Data

Preprocess the data that we web scraped from the previous notebook to prepare it for later analysis. We will prepare two data frames, one to use for exploratory data analysis and one to use to perform a logistic regression model on.

This dataset has 5233 rows and 9 columns. There are 6 non-numerical columns and 3 numerical columns.

OUTPUT: clean_preprocessed_drug_reviews.csv (This dataset has 4,733 rows and 11 columns.)
        preprocessed_drug_reviews_for_lr.csv (This dataset has 4,656 rows and 13 columns.)

----------------------------------
3. Exploratory Data Analysis (EDA)

Create some visualizations to gain insights regarding the distribution of the ratings and the number of reviews.

------------------------------------
4. Natural Language Processing (NLP)

Employ Natural Language Processing (NLP) techniques to see the most common words in the drug reviews. We will use different topic modeling models to identify clusters or groups of similar words within a body of text.

---------------------------------
5. Logistic Regression (Unigrams)

Employ a logistic regression model to find unigrams that are predictive of positive and negative sentiment. We will exclude the drug reviews for Ozempic so that the model does not contain words from that corpus. We will also count the frequency of those words in the Ozempic drug reviews.

--------------------------------
6. Logistic Regression (Bigrams)

Employ a logistic regression model to find bigrams that are predictive of positive and negative sentiment. We will exclude the drug reviews for Ozempic so that the model does not contain words from that corpus. We will also count the frequency of those words in the Ozempic drug reviews.

---------------------------------
7. Logistic Regression (Trigrams)

Employ a logistic regression model to find trigrams that are predictive of positive and negative sentiment. We will exclude the drug reviews for Ozempic so that the model does not contain words from that corpus. We will also count the frequency of those words in the Ozempic drug reviews.
