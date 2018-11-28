# Data analysis Of Yelp reviews :hand: fa18-523-65, fa18-523-67
|Prajakta Patil, Sahithya Sridhar 
| patilpr@iu.edu, sahsrid@iu.edu
| Indiana University, Bloomington
| hid: fa18-523-65, fa18-523-67
| github: [:cloud:](https://github.com/cloudmesh-community/fa18-523-65/blob/master/project-report/report.md)

---

Keywords: Yelp, Natural language processing (NLP), Sentiment analysis, Scikit-learn

---

## Abstract

Yelp is a search service with website that hosts reviews for businesses,
mainly restaurants, that are useful to people looking for one in a city.
Our project performs analysis on text reviews to find how well they correlate
with star ratings given by users to restaurants. It is found that star rating
of 1 and 5 are well correlated with textual reviews. Star rating of 2, 3 and 4
are not so well correlated with textual reviews. This analysis can help users
make better decisions by suggesting them to either just look at star ratings 
or go through actual text reviews.

## Keywords

Yelp, Natural language processing (NLP), Sentiment analysis, Tableau, 
Gephi, Scikit-learn

## Introduction

Users visit Yelp website to either look for a restaurant or write a review for 
one after their visit. Yelp had 148 million reviews on its website at the end 
of 2017. Reviews are in both text and star rating format. Users also post 
pictures of food and restaurant. This helps users looking for restaurants make
decisions. This is also useful to businesses to improve their services. When a
restaurant is very popular, it obviously has more reviews and high star rating.
In such case it is obvious for someone to choose that restaurant if it fits 
their choice of cuisine, budget and other parameters they might have in mind.
However, when there are multiple restaurants that are similar; it becomes 
little difficult to choose one. We took a dataset of Yelp reviews and tried to
find correlations between text reviews and star ratings. We perform additional
analysis to show additional patterns in data. Technologies used to perform 
analysis is Natural Language Processing and Sentiment Analysis.

## Literature review

Li et al performed text analysis on Yelp reviews to study if they can be 
categorized as ‘Useful’. This analysis was needed for businesses that don’t 
have many reviews and hence no reviews categorized as either useful/funny/cool. 
Researchers used SVM and Random Forest models to perform this analysis. They 
extracted features such as number of words, sentences, average sentence length,
TFIDF, star rating, sentiment of review as positive/negative, number of votes 
received by a review, how long has the user been providing Yelp reviews etc. 
Using SVM, researchers were able to achieve accuracy of 0.67 and 0.69 in case
of Random Forest model for predicting if review is ‘Useful’. [@fa18-523-65-www-5]

Hajas et al tried to understand how external factors such as changing taste result
in cyclic behavior for user reviews for restaurants. They took Yelp reviews from 
11 college campuses across USA and modelled restaurant rating as function of 
restaurant quality using a second-degree liner differential function. They were
able to show how restaurant quality results in cyclic behavior for ratings. This
means that restaurants that have good quality, may drop their investment in 
keeping quality constant which results in bad reviews. This in turn forces them
to invest back in quality to gain back lost business. Researchers also created
heat maps to show how restaurants of similar high quality tend to be closer to
each other to gain from bigger crowds. [@fa18-523-65-www-4]

Koven et al focused on methods to predict useful reviews. Their motivation was 
that there is lot of work done in trying to find bad/fake reviews. But, it was
useful to find genuine and useful reviews. They created various attributes for
Yelp reviews such as reviewer’s average star rating, relationship between reviewers,
topic and personality analysis, geographic distribution of reviews etc. They used 
J48 algorithm and reached accuracy of 79.8 in predicting if a review is useful or
not. They were also able to predict bad reviews with roughly 5% false positives.
[@fa18-523-65-www-7]


## Dataset

Dataset used for analysis is taken from Kaggle website. Data contains 5.2 million
user reviews for 174k businesses from 11 metropolitan areas. Data is in CSV and 
JSON format. It has following features business_id, name, neighborhood, address,
city, state, postal_code, latitude, longitude, stars, review_count, attributes,
categories. 

## Data processing

Data is processed to get it ready for analysis. Using NLTK library we removed 
stop-words. We also removed punctuations. All the words are converted to lowercase.
We also removed unnecessary symbols and spaces. We didn’t remove numbers as it might
help users with prices which is an important factor while choosing a restaurant. 
All these operations helped reduce size of data by getting rid of unnecessary data
while retaining useful information.

## Analysis methods

Following methods are used for analysis to make observations and conclusions from 
data:

*	Linear Regression is performed to find if there is any correlation between
reviews and rating (stars). Reviews were characterized into polarity. This is done
using python library called ‘TextBlob’. Polarity value is between -1 to 1. Polarity
above 0 means text emotion is positive while, polarity below 0 means text emotions
are negative. 0 polarity means neutral emotions. We also calculated another parameter
called ‘subjectivity’. Subjectivity reflects user’s personal emotions, opinions.
Subjectivity is between 0 to 1. Subjectivity of 0 means fact-based opinion and 1
means subjective opinion. We also used this method to find if there are correlations
between reviews and classification of review i.e. whether it is categorized as 
‘useful’, ‘cool’ or ‘funny’. As data we worked with was large, we used sampling 
method to use only 10% of all data for this analysis.	
* Logistic Regression, Multinomial Naïve Bayes and Random Forest algorithm These 
are used to predict rating based on text review. This will help understand and 
predict how well text review and ratings match. Low accuracy means there is more
to ratings that just text review. High accuracy means ratings accurately capture
sentiments in text review. 
*	Count, Term Frequency Inverse Document Frequency (tfidf) vectorizer, and Linear
SVC. These help with understanding which words are most commonly used in reviews 
for a restaurant and help gain insight on why certain place might be famous or 
infamous for.
 
## Results

Linear regression between polarity and star ratings showed correlation coefficient is
0.61. This means review emotions and star ratings are moderately correlated. This is 
shown in Fig. 1. We can see regression line graphically represents this correlation 
between review text and star rating given by user. One important result is that we got
p value less than 0.001. Meaning, the results are highly significant and that they are
very unlikely to have occurred by chance. Review classification such as ‘useful’, ‘cool’
and ‘funny’ has negative correlation with review emotions. This is likely because people
might have used ironic language while providing review for a business. All results for 
linear regression analysis are shown in Table. 1. 

**Table. 1 Correlation between review sentiment and star rating and review class**

|      Polarity      | Correlation coefficient | p value |
| (Review Sentiment) |      - r value          |         |                    
|--------------------|-------------------------|---------| 
| Star Rating        |  0.61                   | <0.001  |
| Useful             | -0.064                  | <0.001  |  
| Funny              | -0.043                  | 3.97    |
| Cool               | -0.011                  | 3.66    |
  
We used 3 different machine learning algorithms i.e. Logistic Regression, Multinomial 
Naïve Bayes and Random Forest, to check for accuracy in classifying review into 5 
star-ratings from 1 to 5. Count vectorizer was used to encode data features in a matrix
which these algorithms can learn in scikit-learn. We trained all 3 models on data set 
and checked their performance for guessing rank on test data. Highest overall precision
of 0.55 was achieved with Logistic Regression. All 3 models had higher precision in 
predicting 1 and 5 star ratings and lowest precision in predicting star rating 3 in
general.

**Table. 2 Logistic Regression**

| Star Rating | Precision | Recall  | F1-Score |               
|-------------|-----------|---------|----------| 
| 1           | 0.68      | 0.65    | 0.67     |
| 2           | 0.33      | 0.15    | 0.21     |
| 3           | 0.35      | 0.28    | 0.31     |
| 4           | 0.42      | 0.39    | 0.41     |
| 5           | 0.67      | 0.79    | 0.73     |
| Average     | 0.55      | 0.57    | 0.56     |

**Table. 3 Multinomial Naïve Bayes**

| Star Rating | Precision | Recall  | F1-Score |               
|-------------|-----------|---------|----------| 
| 1           | 0.68      | 0.75    | 0.71     |
| 2           | 0.29      | 0.03    | 0.05     |
| 3           | 0.17      | 0.03    | 0.04     |
| 4           | 0.40      | 0.39    | 0.39     |
| 5           | 0.63      | 0.85    | 0.72     |
| Average     | 0.50      | 0.57    | 0.52     |

**Table. 4 Random Forest**

| Star Rating | Precision | Recall  | F1-Score |               
|-------------|-----------|---------|----------| 
| 1           | 0.54      | 0.55    | 0.54     |
| 2           | 0.47      | 0.07    | 0.12     |
| 3           | 0.23      | 0.11    | 0.15     |
| 4           | 0.33      | 0.25    | 0.28     |
| 5           | 0.59      | 0.82    | 0.68     |
| Average     | 0.47      | 0.51    | 0.47     |

We created confusion matrix to understand these correlations in simpler way.
We grouped our data by star rating. Confusion matrix thus created is shown in
form of heatmap in Fig. 2. We can see that ‘useful’ and ‘funny’ is correlated
with text length. ‘cool’ and ‘subjectivity’ are correlated to polarity.

![Fig. 2. correlation heat map](images/Fig 2.PNG){#fig:fig2}

We wanted to understand patterns from this data. First, we looked at reviews by
states. Shown in Fig. 3, we see Arizona is the state with most reviews for 
businesses followed by Nevada and California. We then looked at number of reviews
by cities. As seen in Fig. 4, Las Vegas is the city with most number of reviews 
with 26775 reviews followed by Phoenix and Toronto. Fig. 4 shows only top 20 cities
but, our dataset has reviews for 11 metropolitan areas and had reviews for 1093 
cities. We also looked at what type of businesses are present on Yelp. In Fig. 5 
we can see that various types of restaurants receive most reviews followed by
shopping and home services. Another interesting observation we wanted to make was
which weekday was preferred by users to go out and hence provide reviews for these
businesses. Fig. 6 shows that most users liked to go out on Saturday followed by 
Sunday and Friday. Monday and Tuesday saw lowest number of checkins for businesses.

Insert Fig. 3, 4, 5 and 6 here.

![Fig. 3.](images/Fig 3.PNG){#fig:fig3}
![Fig. 4.](images/Fig 4.PNG){#fig:fig4}
![Fig. 5.](images/Fig 5.PNG){#fig:fig5}
![Fig. 6.](images/Fig 6.PNG){#fig:fig6}

We used pandas’ ‘groupby’ function to calculate mean star ratings for businesses.
For purpose of this project we decided to look at details of restaurants only. 
Fig. 7 shows top rated restaurants with descending average descending star rating.
We are showing top 20 businesses only as data has more than 1000 places. ‘Earl of 
Sandwich’ was top rated restaurant with average rating of 4.25. Top 10 places are
dominated by restaurants that serve pizza and burger. One other thing to notice is
that most of these restaurants are franchises. However, regional franchises have 
higher star ratings than ones that have pan US presence.

![Fig. 7.](images/Fig 7.PNG){#fig:fig7}

Fig. 8 shows distribution of ratings offered to businesses. We see that rating 5 
was most used rating by reviewers for describing their experience at given restaurant.
Rating 2 was least used rating. Looking at distribution of review length for each star
rating shows there was no significant difference in review length distribution. 
However, comparing Fig. 9 with Fig. 8 shows same trend. Meaning more restaurants got
5-star rating but they also got some textual review. We also looked average number 
of reviews given by users. We can see in Fig. 10 that most users provided less than
5 reviews. There is small percentage of users who have provided more than 30 reviews.

![Fig. 8.](images/Fig 8.PNG){#fig:fig8}
![Fig. 9.](images/Fig 9.PNG){#fig:fig9}
![Fig. 10.](images/Fig 10.PNG){#fig:fig10}

We were interested in seeing usage of words to describe user experience about a certain
place. We chose 11 words that we thought could have been most used in reviews. This list
covered words that help express both positive and negative emotions. Fig. 11 shows that
word ‘great’ was used a lot by users to describe positive experience. Word ‘bad’ was 
used mostly to describe negative experience.

![Fig. 11.](images/Fig 11.PNG){#fig:fig11}

## Discussion

We observed higher accuracy in predicting star rating of 1 and 5 than all other ratings
i.e. 2, 3 and 4. This was one limitation that we think is result of understanding user
emotions and applying language model to decode it. It is difficult to find how many users
write a very objective review and give star rating accordingly. It is possible that 
someone has either a better or worse than expected experience and provides a review based
purely on emotions at that point of time. Additional analysis on understanding how a 
person from certain cultural background finds food from other cultures.

## Conclusions

We have been able to show textual review and star rating are generally moderately correlated.
If a user wishes to choose a business for visiting such as choosing a restaurant for eating 
out, they can look at rely more on star rating 4 and  to find a good place and star rating 1
to know that a certain place is bad. If the restaurant has star rating of 2 or 3, they will
have to spend more time in reading the actual textual reviews to make their decision. A good 
business has lot more reviews than a bad business. Most users give very few reviews and they
do so more in case if their experience was good. Businesses serving pizzas and burgers are 
one of most liked places.

## Project members and Work Breakdown

Prajakta Patil - fa18-523-65: Introduction, Literature review, Dataset
Sahithya Sridhar- fa18-523-67: Abstract, Data processing, Analysis methods

