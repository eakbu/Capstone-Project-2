# Capstone-Project-2# NLP Sentiment Analysis on Health and Personel Care Products

## Introduction
The company wants to develop a software tool that will identify the positive and negative words which customers use when they write reviews for the health and personal care products as their purchase inclination. For that, they gave their 9 years health and personal care products’ reviews between 2004-2014 and asked us to develop a model which will identify positive and negative words used in the reviews as a component of customer’s sentiment towards to the company’s health and personal care products. 

## Data

The data is in Standford Analysis Project (SNAP) webpage. The original data was in a JSON format there. In order to analyze the data, I imported JSON package and decoded JSON file with using query in order to convert JSON file to csv file format. The original dataset for this project can be found [here](http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Health_and_Personal_Care_10.json.gz)

## Data Wrangling
  Data insection and text preprocessing is completed in this section. It can found [here](https://github.com/eakbu/Capstone-Project-2/blob/main/data%20wrangling/amazon%20health%20and%20personal-care%20sentiment%20analysis.ipynb)

## Exploratory Data Analysis
Univarate and bivariate analysises are done by using bar charts and wordcloud visualizations. These analysis can be found [here](https://github.com/eakbu/Capstone-Project-2/blob/main/data%20storytelling/Exploratory_Data_Analysis_for_Sentiment_Analysis.ipynb)

## Modeling
This is a supervised binary classification problem. We are trying to predict the sentiment based on the reviews left by females who bought health and personal care products in Amazon e-commerce online platform. I used Python’s Scikit Learn libraries to solve the problem. In this context, we implemented Logistic Regression, Random Forest,and  Naive Bayes algorithms. 
Since the ratings of the reviews were not distributed normally, we decided to decrease rating classes from 5 to 2 by merging Rating 1-2 as ‘Bad’ and Rating 4-5 as 'Good' while dropping Rating 3 from the dataset.
For feature selection, we applied threshold for word occurrence with using min_df/max_df. For feature engineering, I applied CountVectorizer, TF-IDF, and Hashing Vectorizer to the text data in order to turn a collection of text documents into numerical feature vectors. 

Modeling notebooks can be reached from following links. 

- [Count Vectorizer, TF-IDF, Hashing Vectorizer with Traditional Algorithms](https://github.com/eakbu/Capstone-Project-2/blob/main/data%20feature%20selection%20and%20model%20building/feature%20selection%20and%20model%20building.ipynb)
- [Threshold for word occurence, SMOTE techniques used with Traditional Algorithms](https://github.com/eakbu/Capstone-Project-2/blob/main/data%20feature%20selection%20and%20model%20building/feature%20selection%20and%20model%20building-model%20performance%20improvement.ipynb)

## Conclusion
Report can be found [here](https://github.com/eakbu/Capstone-Project-2/blob/main/mile%20stone%20report/capstone%202%20mile%20stone%20report%20%20final.pages)
