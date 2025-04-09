# IMDb Movie Review Sentiment Prediction using LSTM

## Overview
This project uses a deep learning model based on Long Short-Term Memory (LSTM) networks to predict the sentiment of IMDb movie reviews. Given a review in plain text, the model classifies it as either positive or negative. It demonstrates how natural language processing (NLP) and sequential models can automate opinion analysis from large-scale user-generated content.

## Problem Statement
With thousands of reviews posted on platforms like IMDb every day, manual sentiment analysis becomes impractical. These reviews, however, carry valuable insights that can help viewers, content creators, and marketers understand public opinion.

The objective of this project is to build a model that can automatically detect the sentiment of a movie review using deep learning techniques. Specifically, it aims to:

- Train a model that captures both the semantics and sequence of words in a review.
- Predict the sentiment class (positive or negative).
- Evaluate the model's performance using relevant metrics.

## Dataset
- Source: IMDb Movie Review Dataset
- Total Samples: 50,000
- Train/Test Split: 25,000 for training and 25,000 for testing
- Sentiment Classes: Binary (Positive and Negative)
- Balanced: Yes

## Methodology

1. **Text Preprocessing**
   - Tokenize the review text
   - Convert words into integer sequences
   - Apply padding to ensure uniform input length

2. **Model Architecture**
   - Embedding layer to convert words into dense vectors
   - LSTM layer to process the sequence data
   - Dense layer with sigmoid activation for binary classification

3. **Training Setup**
   - Loss Function: Binary Crossentropy
   - Optimizer: Adam
   - Metrics: Accuracy

4. **Evaluation**
   - Use test data to evaluate model performance
   - Generate classification report and confusion matrix

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## Results
The model achieved high accuracy on the test set, demonstrating its ability to learn sentiment patterns from textual data. The goal of reaching at least 85% accuracy was met, and additional metrics further confirmed the model’s effectiveness.

## How to Run

1. Clone or download this repository.
2. Install the required libraries:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn tensorflow
