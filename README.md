# Capstone_Project_03_Corona-virus-Tweet-Sentiment-Analysis

Author:  Pankaj R. Beldar
Email: pankajrbell@gmail.com


# Contribution:

This project is based on Natural Language Processing and Aim is to classify the sentiment of Covid 19 Tweets so that it can be used for different stakeholders. I have done Data Preprocessing ,Text Cleaning, Exploratory Data Analysis, Vectorization, Implementing  Multiclass Classification Models,  Hyperparameter tuning, Binary Classification Models, Stacking, Voting Algorithms to increase model accuracy.

# Data Cleaning-

Removed @users from tweets
Removed Punctuations
Removed Stopwords
Removed HTML tags
Removed URLs
Removed Short words
Removed Emojies
Convert text to Lower Case
Stemming
Tokenizing
Spelling Correction

# Exploratory Data Analysis

How many Tweets per day for the given time period?
Which are the Top 30 Locations from where maximum tweets were done?
What are the Sentiment types and its Distribution?
What is the relationship between the number of words, characters, sentences and different types of Sentiments?
What are the most frequent Extremely Positive Sentiment Words?
What are the most frequent Positive Sentiment Words?
What are the most frequent Extremely Negative Sentiment Words?
What are the most frequent Negative Sentiment Words?
What are the most frequent Neutral Sentiment Words?
Finding out top 10 most frequent words based on sentiment.

![download (16)](https://user-images.githubusercontent.com/111692879/202973956-98a42450-de9a-46ed-960a-7d1b52c2db0e.png)


![download (17)](https://user-images.githubusercontent.com/111692879/202973998-d8941a68-6bf8-4030-ae45-18232154e60d.png)


![download (14)](https://user-images.githubusercontent.com/111692879/202974104-84e592cf-6cbf-410d-a43a-c7aa1a8b2d5e.png)


# vectorization

Countvectorizer
Tfidfvectorizer
N-grams vectorizer

# Classification Models used:
Stacking Classifier
Stochastic Gradient Descent Classifier
Voting Classifier 
CatBoost Classifier
Extra Tree Classifier
Support Vector Classifier
Random Forest Classifier
Multinomial Naive Bayes Classifier
XGboost classifier.

![download (19)](https://user-images.githubusercontent.com/111692879/202974549-0c649408-32cf-48ee-bdb3-fa2c39f1c5f7.png)


![download (18)](https://user-images.githubusercontent.com/111692879/202974471-b195cba6-8d85-4921-9eb8-77e6ab6cc3b9.png)


# Useful Links-

Github Link: - https://github.com/pankaj-beldar/Capstone_Project_03_Corona-virus-Tweet-Sentiment-Analysis

Google Drive Link:- https://drive.google.com/drive/folders/1QSN4tLcTWYURTvMFoNq7zOQmOsydgNjK?usp=sharing

Project Title:- Sentiment Analysis : Predicting Sentiment of COVID-19 tweets


# Summary of your Capstone project:

I have tried Stacking classifier, Stochastic Gradient Descent Classifier, voting, CatBoost, Extra Tree, Support Vector Classifier, Random Forest Classifier, Multinomial Naive Bayes and XGboost classifier.

I have Extracted new Features as number of words, characters and sentences to check sentiment of the Tweet.We can see that if the number of words, characters and sentences are more than sentiment of the tweet is more positive. Neutral Sentiment Tweets consist of fewer words, characters and sentences. After evaluating models with these features we have found that these features are not contributing much in the model performance. Hence we have decided to drop them in Binary classification models

Firstly I have evaluated the multi class models as categories -Positive, Extremely Positive, Neutral, Negative, Extremely Negative. Most of the people (28% ) were having Positive sentiment about covid followed by Negative (24%), Neutral(19%), Extremely Positive (16%) and Extremely Negative(13%). Our Target variable is not Unbalanced as all Categories are not having much differences between them.

The performance of the Multiclass Models is not satisfactory then we convert the problem into binary class. We have kept only two Sentiments as Positive and Negative.
The Binary Stacking Classifier has the best performance of accuray 0.8650  followed by CatBoost and Extra Tree classifier.

I have checked for Voting classifiers and Stacking Classifiers with hyperparameter tuning.
For vectorizing I have tried all kinds of vectorizing methods i.e. tfidfvectorizer ,countvectorizer, ngrams, after doing hyper parameter tuning,I have decided to use countvectorizer for vectorization.

Sentiment Analysis is done based on Positive and Negative Sentiment.

As we are dealing with sentiment analysis of coronavirus tweets, It's very important to classify sentiment as either positive or negative to use it as reference for different stakeholders. Governments can make use of this information in policymaking as they are able to know how people are reacting to this new strain, what all challenges they are facing such as food scarcity, panic attacks, etc. Various profit organizations can make a profit by analyzing various sentiments as one of the tweets tells us about the scarcity of masks and toilet papers. These organizations are able to start the production of essential items thereby making profits. Various NGOs can decide their strategy of how to rehabilitate people by using pertinent facts and information.We could do the analysis with three classes as positive, negative and neutral.

