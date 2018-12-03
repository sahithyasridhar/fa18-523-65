

# Data analysis Of Yelp reviews

| Authors: *Sahithya Sridhar, Prajakta Patil*

We have divided the project into two parts. In the first part, we visualize and analyze the data. In the second part, we use split the data into train and test data and use various machine learning algorithms to determine how the test data performs with our machine learning model.

## Data

The data set is downloaded from

```
kaggle datasets download -d yelp-dataset/yelp-dataset

```
It contains the following files that we used for our analysis:

* yelp_business.csv - This is the data file which is located in the below mentioned folder:
This file contains information about the business like business_id, name of the business, postal code, number of stars for the business, review count, category of the business etc.
* yelp_review.csv - This file contains information about the user reviews like user_id, business_id, date of the review, usefulness of the reviews etc.
* yelp_tip.csv
* yelp_checkin.csv.

## Requirements

These are the main requirements to setup and run the code.
  1. Python 3
  2. 	import nltk
	    nltk.download()


## Installation

We got the dataset files in the csv format from the kaggle website. If the data set file is in any other format say JSON for example, we need to conver it to CSV.

The following python packages need to be installed before we can run the code in the Jupyter Notebooks. 

     ```python
     pip install jupyter
     pip install scipy
     pip install numpy
     pip install pandas
     pip install sklearn
     pip install matplotlib
     pip install seaborn
     pip install wordcloud
     pip install geopy
     pip install plotly
     pip install cufflinks
     conda install basemap
     
      ```
6. Run the Code files in the following order:

   6.1. **Exploratory Analysis of Yelp data set.ipynb**
   
   6.2. **Machine Learning analysis of yelp data set.ipynb**
