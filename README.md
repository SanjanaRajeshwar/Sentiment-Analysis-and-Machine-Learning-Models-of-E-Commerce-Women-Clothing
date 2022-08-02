# Sentiment-Analysis-and-Machine-Learning-Models-of-E-Commerce-Women-Clothing
# OBJECTIVE:
This project proposes a sentiment analysis model for analyzing positive-negative customer reviews for E-Commerce Women's Clothing. From an e-commerce standpoint today, customer behavior research is gaining significant importance as consumers are shifting from visiting retail stores to shopping online. There is strong need to understand customer feedback with accuracy and apply it improve the product and services by sellers.
In this project, customer reviews of E-Commerce Women's Clothing were used to evaluate, implement, and analyze the effective strategies in context of sentiment analysis.   
Various classification models (machine learning and deep learning) were analyzed along with sentiment analysis. The best model was identified based on the parameter of accuracy along with precision, recall, f1-score, and support.
# DATASET:
The dataset that we used is Women’s Clothing E-Commerce from Kaggle that consists of reviews from real end consumers and hence the details and information regarding the customer and company has been anonymized or replaced. This dataset 11 columns, with each row representing a customer review.
# DATA PREPROCESSING:
First, all the columns were checked for null values. If any column had more than 80 percent null values, the column was dropped/ removed. All the columns were renamed as space between column names was replaced with underscore for coding convenience. Also, data rows with null values in review text column were removed. Columns like unnamed_0, clothing_id which mostly had unique values and were not of any use of us were also dropped. Also, some of the reviews with these ratings given by the user suggested that the user would recommend the cloth but they didn’t and vice-versa.
# TEXT PREPROCESSING:
First, tokenization was performed which broke the raw text into words, sentences called tokens. Then, punctuations like full stop, comma, hyphen, colon, etc were removed. Stop words like I, am, is, had, etc. were also removed as such words do not add any meaning to text and removing them reduces noise and dimension of the feature set. Then lemmatization was done which combined a word's several inflected forms into a single item that can be analyzed easily. Lemmatization was chosen over stemming as it brings context to the words.
# SENTIMENT ANALYSIS:
Next, I classified each review as negative or positive with the help of VADER (Valence Aware Dictionary and Sentiment Reasoner) module which is a tool that measures the amount of positive and negative emotion in a text as well as the intensity of that emotion.
# FEATURE EXTRACTION METHOD:
CountVectorizer is a very important tool provided by scikit-learn. Library of python that is used to convert a given text into a vector based on the frequency (count) of each word that appears throughout the text.
# TRAIN TEST SPLIT:
Cleaned review text were taken as x and recommended column was taken as y. For MACHINE LEARNING models, the train test split with a test size of 30% was taken.
# CLASSIFICATION MODELS:
Six classification machine learning models were built to predict whether the clothing piece is recommended by the customer based on the review given by them.
->Multinomial Naive Bayes
->Support Vector Machine
->Random Forest Classifier
->Neural Network Model
->Ada Boosting Classifier
->K Nearest Neigbour
