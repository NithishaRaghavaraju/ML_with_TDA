

# Machine Learning with Topological Data Analysis (TDA)

## Overview

This project integrates Machine Learning (ML) and Topological Data Analysis (TDA) to develop a chatbot system. The chatbot leverages NLP techniques, word embeddings, and persistence diagrams from TDA to enhance text classification. The model processes user queries, extracts word embeddings using FastText, applies TDA to analyze sentence structure, and predicts an appropriate response using a neural network.

## Features

Natural Language Processing (NLP): Preprocessing of text data, tokenization, and word embeddings (Word2Vec, FastText).

Dimensionality Reduction: PCA applied to embeddings for visualization and feature optimization.

Topological Data Analysis (TDA): Uses Gudhi library to extract persistence diagrams and persistence landscapes.

Neural Network Model: A sequential model with dense layers, layer normalization, and dropout for text classification.

End-to-End Pipeline: From text processing to chatbot response generation.

## Structure

### Data Processing:

Loads JSON file into Pandas DataFrame.

Tokenizes text and encodes labels.

Applies FastText for word embeddings.

TDA Feature Extraction:

Constructs Rips Complex.

Computes persistence diagrams.

Transforms diagrams into persistence landscapes.

### Neural Network Model:

Uses concatenated sentence embeddings and TDA features.

Trains a sequential deep learning model for classification.



