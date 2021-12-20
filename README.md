
# Clubhouse App Analysis

Mentioned below is a concise guide to the the steps we followed while working on this project.

## Step 1 - Market Research

Here is a list of links that we referred to for market research

1.  [Basic information](https://www.thinkimpact.com/clubhouse-statistics/)  and  [statistics](https://www.thinkimpact.com/clubhouse-statistics/2)  about Clubhouse
2.  [App ranking in iOS](https://app.sensortower.com/ios/US/alpha-exploration-co/app/clubhouse/1503133294/category-rankings?category=0&start_date=2014-01-01&end_date=2021-12-05&countries=US&chart_type=free&device=iphone&hourly=false&selected_tab=charts&date=2021-09-07&summary_chart_type=topfreeapplications): Above Data revealed Clubhouse faced a challenge as its app store ranking dropped significantly in March
3.  [Competitor analysis](https://trends.google.com/): We used the library called [pytrends](https://pypi.org/project/pytrends/) and [GoogleNews](https://pypi.org/project/GoogleNews/) present in python to scrap keyword search volumes and news articles in Google. Clubhouse's competitors were planning to launch similar apps and customers interest from keyword search volume also demonstrates other apps are getting more popular, meanwhile Clubhouse is in the opposite direction.

## Step 2 - Review scraping from Google Playstore

We used the library called  [google_play_scraper](https://pypi.org/project/google-play-scraper/)  present in python to help us with the scraping. The modules imported were ‘Sort’, ‘reviews’ and ‘app’. The ‘reviews’ module was fruitful in providing us with the data we needed. This  [website](https://python.plainenglish.io/scraping-storing-google-play-app-reviews-with-python-5640c933c476)  proved to be helpful to us in the coding part. We have submitted a Jupyter notebook named reviews_scraper.ipynb which has the code for scraping.

## Step 3 - T-test

Here are a few links that can help in the conceptual understanding of t-test.  [Link1](https://www.investopedia.com/terms/t/t-test.asp)  [Link2](https://www.jmp.com/en_us/statistics-knowledge-portal/t-test/two-sample-t-test.html)  T-test was conducted in minitab. Below are the steps to be followed

1.  Copy the two columns of data whose averages you want to compare.
2.  Go to Taksbar. Stat--> Basic Statistics--> 2 sample t-test. A dialog box opens up.
3.  Choose your columns
4.  Then click on 'Options' in the same dialog box. Choose your significance level and the hypothesis you want to test.
5.  Click Ok. You will now be able to see the results.

Interpretation of results :

-   If p-value <  **α**  --> Reject Null Hypothesis
-   If p-value >  **α**  --> There is not sufficient evidence to reject Null Hypothesis.


## Step 4 - LDA Topic Modelling

-   **Latent Dirichlet allocation** (**LDA**) is a “generative statistical model” that allows sets of observations to be explained by unobserved groups that explain why some parts of the data are similar. So this is categorized as unsupervised learning. For example, if observations are words collected into documents, it posits that each document is a mixture of a small number of topics and that each word’s presence is attributable to one of the document’s topics. LDA is an example of a [topic model.](https://en.wikipedia.org/wiki/Topic_model)
    
-  We used the library called [LatentDirichletAllocation](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.LatentDirichletAllocation.html) present in python to help us find out the topics which are occuring most prominently in the document. For pre-processing the text reviews we have used the [nltk.tokenize](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.LatentDirichletAllocation.html) and [nltk.stem.lemmatize](https://www.nltk.org/_modules/nltk/stem/wordnet.htmllibraries ) python libraries for tokenizing and lemmatizing the document. Finally, we have submitted a Jupyter notebook named lda_codesetup.ipynb which has the code for scraping.
   
- To reproduce the results, kindly upload the file to Jupyter before running the code.
----------

**Contributors**: * Manideep Sharma * Mrinmayee Joshi * Lakshay Vohra * Jaemin Kim

