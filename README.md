# natural_language_processing
## Description
This project implements a classification model to perform sentiment analysis on restaurant reviews. The process begins with text cleaning, creating a Bag of Words model, and using **CatBoostClassifier** to predict whether a review is positive or negative.

## Dataset
The dataset used is `Restaurant_Reviews.tsv`, which contains text reviews and binary labels indicating whether the review is positive or negative. The dataset consists of 1000 reviews.

## Languages or Tools
- Python
- Jupyter Notebook or any Python platform

## Libraries
- `pandas`
- `numpy`
- `matplotlib`
- `nltk`
- `sklearn`
- `catboost`

## Algorithm Overview
The project performs text cleaning using stemming with PorterStemmer and removes insignificant common words (stopwords). Afterward, the Bag of Words model is used to convert the text into numerical representation. Next, the **CatBoostClassifier** model is used to train the data and predict the sentiment of the reviews.

Steps:
1. **Text Cleaning**: Removing non-alphabet characters, converting to lowercase, and applying stemming.
2. **Bag of Words**: Creating a numerical representation of the text using `CountVectorizer` with a maximum of 1500 features.
3. **Dataset Splitting**: Splitting the dataset into training and test sets with an 80:20 ratio.
4. **Model Training**: Training the **CatBoostClassifier** model using the training data.
5. **Model Evaluation**: Using confusion matrix and accuracy score to evaluate model performance.
