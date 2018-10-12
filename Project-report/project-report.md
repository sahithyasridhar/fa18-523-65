Data analysis Of Yelp revievs
======
# Work Breakdown:

Prajakta Patil - fa18-523-65: Introduction, Literature review, Dataset

Sahithya Sridhar- fa18-523-67: Abstract, Data processing, Analysis methods

# Abstract:
Yelp is a search service with website that hosts reviews for businesses, mainly restaurants, that are useful to people looking for one in a city. Our project performs analysis on text reviews to find how well they correlate with star ratings given by users to restaurants. This analysis can help users make better decisions by suggesting them to either just look at star ratings or go through actual text reviews. We also looked for various patterns in the data to see which factors affect reviews and ratings. 
# Keywords:
Yelp, Natural language processing (NLP), Sentiment analysis, Tableau, Gephi, Scikit-learn
# Introduction:
Users visit Yelp website to either look for a restaurant or write a review for one after their visit. Yelp had 148 million reviews on its website at the end of 2017. Reviews are in both text and star rating format. Users also post pictures of food and restaurant. This helps users looking for restaurants make decisions. This is also useful to businesses to improve their services. When a restaurant is very popular, it obviously has more reviews and high star rating. In such case it is obvious for someone to choose that restaurant if it fits their choice of cuisine, budget and other parameters they might have in mind. However, when there are multiple restaurants that are similar; it becomes little difficult to choose one. We took a dataset of Yelp reviews and tried to find correlations between text reviews and star ratings. We also tried to show hidden patterns present in this data. We use Tableau and Gephi to visualize the data which helps gain valuable insights and suggest what detail analysis might be useful. Technologies used to perform analysis is Natural Language Processing and Sentiment Analysis. 
# Literature review:
Li et al performed text analysis on Yelp reviews to study if they can be categorized as ‘Useful’. This analysis was needed for businesses that don’t have many reviews and hence no reviews categorized as either useful/funny/cool. Researchers used SVM and Random Forest models to perform this analysis. They extracted features such as number of words, sentences, average sentence length, TFIDF, star rating, sentiment of review as positive/negative, number of votes received by a review, how long has the user been providing Yelp reviews etc. Using SVM, researches were able to achieve accuracy of 0.67 and 0.69 in case of Random Forest model for predicting if review is ‘Useful’.[@fa18-523-65-www-5]

Hajas et al tried to understand how external factors such as changing taste result in cyclic behavior for user reviews for restaurants. They took Yelp reviews from 11 college campuses across USA and modelled restaurant rating as function of restaurant quality using a second-degree liner differential function. They were able to show how restaurant quality results in cyclic behavior for ratings. This means that restaurants that have good quality, may drop their investment in keeping quality constant which results in bad reviews. This in turn forces them to invest back in quality to gain back lost business. Researchers also created heat maps to show how restaurants of similar high quality tend to be closer to each other to gain from bigger crowds.[@fa18-523-65-www-4]

Koven et al focused on methods to predict useful reviews. Their motivation was that there is lot of work done in trying to find bad/fake reviews. But, it was useful to find genuine and useful reviews. They created various attributes for Yelp reviews such as reviewer’s average star rating, relationship between reviewers, topic and personality analysis, geographic distribution of reviews etc. They used J48 algorithm and reached accuracy of 79.8 in predicting if a review is useful or not. They were also able to predict bad reviews with roughly 5% false positives.[@fa18-523-65-www-7]
# Dataset:
Dataset used for analysis is taken from Kaggle website. Data contains 5.2 million user reviews for 174k businesses from 11 metropolitan areas. Data is in CSV and JSON format.  It has following features business_id, name, neighborhood, address, city, state, postal_code, latitude, longitude, stars, review_count, attributes, categories. 
# Data processing:
Data is processed to get it ready for analysis. Using NLTK library we remove stop-words.  We also remove punctuations. Then we tokenize and stemm words from review texts. All the words are converted to lowercase. We also remove unnecessary symbols and spaces. We don’t remove number as it might help users with prices which is an important factor while choosing a restaurant.  All these operations help reduce size of data by getting rid of unnecessary data while retaining useful information. 
# Analysis methods:
Following methods are used for analysis to make observations and conclusions from data.
1. Logistic Regression, Multinomial Naïve Bayes and Random Forest algorithm
	These are used to predict rating based on text review. This will help understand and predict how well text review and ratings match. Low accuracy means there is more to ratings that just text review. High accuracy means ratings accurately capture sentiments in text review.
2. Count, Term Frequency Inverse Document Frequency (tfidf) vectorizer, and Linear SVC
	These help with understanding which words are most commonly used in reviews for a restaurant and help gain insight on why certain place might be famous or infamous for.
3. Centrality measurements
a)	Degree centrality
b)	Closeness centrality
4. Community detection
	Both centrality measurements and community detection help finding various patterns in network. This can reveal how and if which type restaurant tends to get higher/lower rating depending on its distance from downtown or geographical location etc. 
