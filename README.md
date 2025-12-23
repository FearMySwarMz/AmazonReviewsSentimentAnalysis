# Sentiment Analysis on Amazon Mobile Reviews (Word2Vec & GloVe)

This repository contains a sentiment analysis pipeline on the **Amazon Unlocked Mobile** reviews dataset, implemented in a single Jupyter notebook (`Untitled8.ipynb`). The goal is to predict review sentiment (positive vs negative) from free-text reviews using both Word2Vec and GloVe embeddings combined with traditional machine learning classifiers.[file:1]

## Project Overview

The workflow in the notebook includes:[file:1]

- Loading the `Amazon_Unlocked_Mobile.csv` dataset.
- Basic exploration of product, brand, price, rating and text review fields.
- Text cleaning and preprocessing on the `Reviews` column.
- Tokenization of cleaned reviews.
- Training a **Word2Vec** model (gensim) on the tokenized corpus.
- Loading / using **GloVe** pre-trained word embeddings.
- Creating fixed-size review embeddings:
  - Averaging Word2Vec word vectors per review.
  - Averaging GloVe word vectors per review.
- Constructing binary sentiment labels from the `Rating` column  
  - Ratings 4–5 → positive  
  - Ratings 1–3 → negative.
- Splitting embeddings and labels into train and test sets.
- Training machine learning classifiers on both Word2Vec- and GloVe-based embeddings.
- Evaluating performance with appropriate metrics (e.g. accuracy, confusion matrix, classification report). [file:1]

## Technologies Used

- Python
- Jupyter / Google Colab
- pandas for data handling
- gensim (Word2Vec)
- GloVe pre-trained embeddings
- NumPy / SciPy
- scikit-learn for model training and evaluation[file:1]


1. Clone the repository:
