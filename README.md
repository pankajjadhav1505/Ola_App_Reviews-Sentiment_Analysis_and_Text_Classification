**🚖 Ola App Reviews – Sentiment Analysis & Text Classification**

_A Natural Language Processing (NLP) project using real user reviews._


**Project Overview :**

This project analyses genuine Ola mobile app reviews scraped from the Google Play Store. These reviews capture real customer experiences related to booking, pricing, app usability, payment issues, driver behaviour, and service quality.
The goal of this project is to build a sentiment analysis and predictive machine learning model that can classify user feedback and help understand overall customer satisfaction.
________________________________________

**Dataset Description :**

	Dataset Source - Kaggle
	Dataset Name - Ola Ride Reviews Dataset: Sentiments & Ratings
	Dataset link - https://www.kaggle.com/datasets/sonalshinde123/ola-ride-reviews-dataset-sentiments-and-ratings
	
	The dataset contains real-world user reviews, including:
	•	Review Id
	•	User Ratings (1–5 stars)
	•	Review Text
________________________________________

**Project Objectives :**

	•	Clean and preprocess the raw text data.
	
	•	Perform EDA on customer sentiments and explore review trends, rating patterns using visualizations.
	
	•	Encode text using NLP techniques
	
	•	Build ML models for sentiment classification
	
	•	Create a prediction function to classify new reviews
________________________________________

**Tech Stack :-**
		•	Python
		
		•	Pandas, NumPy
		
		•	Matplotlib, Seaborn, WordCloud
		
		•	Scikit-learn
		
		•	NLTK / Text Preprocessing
________________________________________

**Steps Performed in the Project :**

	1.	Data Preprocessing -
	•	Cleaning text (lowercasing, punctuation & stopwords removal)
	•	Tokenization
	•	Lemmatization
	•	Handling missing values and irrelevant characters.
	
	2.	Exploratory Data Analysis (EDA) -
	•	Rating distribution
	•	Most frequent positive & negative words
	•	WordCloud generation
	•	Review length analysis
	
	3.	Feature Engineering -
	•	TF-IDF Vectorization
	•	Sentiment Label Creation (Positive / Neutral / Negative)
	•	Oversampling minority classes using Random Oversampling

	4.	Model Implementation -
	•	Train/test split
	•	Logistic Regression
	•	Random Forest
	•	Support Vector Machine (SVM)
	•	Model evaluation using:
		o	Accuracy
		o	Precision
		o	Recall
		o	F1-score
		o	Confusion Matrix
	
	5.	Prediction Function -
	A reusable function is created to accept any text review and return:
	Sentiment: Positive / Neutral / Negative
________________________________________

**Results :**

Model Performance Summary: -

Linear SVM was chosen because it provided the most balanced performance across all sentiment classes and was the only model able to predict the Neutral class. While Logistic Regression had slightly higher accuracy, Linear SVM handled class imbalance better, making it the most reliable model overall.

	
Confusion Matrix Insights: -

•	Major misclassifications occurred between Neutral ↔ Positive categories.
	
•	Negative reviews were classified more accurately due to strong emotional word



Key Observations: -	

•	SVM performed the best overall due to high-dimensional text features.
	
•	Random Oversampling significantly improved Recall for minority (neutral/negative) classes.
	
•	Logistic Regression also provided stable and interpretable results.
________________________________________
