# Next Word Recommender using N-grams

# Project Overview

This project focuses on building a Next Word Recommendation system using the Reuters dataset. The system employs n-gram language models (unigram, bigram, and trigram) to predict the next word based on the previous words. The model is trained on a sample dataset containing 10,000 sentences extracted from Reuters news articles.

# Dataset Description

Dataset Name: sample_reuters_dataset.csv

Columns:

Sentence Number: The index of the sentence in the dataset.

Text: The sentence text.

Statistics:

90 different document categories

7,769 training documents

54,716 sentences in total (sample dataset contains 10,000 sentences)

# Project Objectives

Create a vocabulary from the dataset.

Generate unigrams, bigrams, and trigrams from the dataset.

Build a trigram language model that predicts the probability of the next word given two preceding words.

# Implementation Steps

1. Data Preprocessing

Load the dataset.

Tokenize sentences into words.

Convert all words to lowercase.

2. N-gram Model Construction

Generate unigrams, bigrams, and trigrams.

Store frequency counts for each n-gram.

Compute probabilities for each trigram using Maximum Likelihood Estimation (MLE).

3. Next Word Prediction

Given two words as input, use the trigram model to predict the most probable next word.

If a trigram is not found, fall back to bigram or unigram probabilities.

Technologies Used

Python

Pandas (for data handling)

Collections (for frequency distribution)

NumPy (for probability calculations)


# How to Run the Project

Clone the repository:

git clone https://github.com/your-repo/Next-Word-Recommender-using-N-grams
.git
cd next-word-recommender

Install dependencies:

pip install -r requirements.txt

# Expected Output

The application will provide an input box where users can type words.

Based on the input, the system will suggest the most probable next word.

If no trigram match is found, the model will suggest based on bigram or unigram probabilities.

# Future Enhancements

Implement a deep learning-based language model (e.g., LSTMs or Transformers).

Use larger datasets for better accuracy.

Optimize computational efficiency using smoothing techniques.

# Author

Provided by Analytics Vidhya. Implemented by Umunnakwe Tochukwu Precious.
