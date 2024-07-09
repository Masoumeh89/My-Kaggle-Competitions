# Kaggle Competition: Natural Language Processing with Disaster Tweets

## Overview
This repository contains my solution to the Kaggle competition "Natural Language Processing with Disaster Tweets." The objective of the competition is to build a machine learning model that predicts whether a given tweet is about a real disaster or not.

## Competition Description
In this competition, you are challenged to create a model that can distinguish between tweets about real disasters and non-disaster tweets. The dataset contains 10,000 tweets that have been hand-labeled as either disaster-related (1) or not (0).

## Data Description
The dataset consists of the following files:
- `train.csv`: The training set containing tweets labeled as disaster or not.
- `test.csv`: The test set for which you need to predict whether each tweet is about a real disaster.
- `sample_submission.csv`: A sample submission file in the correct format.

Each tweet in the training and test sets contains:
- `id`: A unique identifier for each tweet.
- `text`: The text of the tweet.
- `location`: The location from where the tweet was sent (may be blank).
- `keyword`: A keyword from the tweet (may be blank).
- `target`: (Only in `train.csv`) Denotes whether a tweet is about a real disaster (1) or not (0).

## Approach
### Data Preprocessing
1. **Text Cleaning**: Removed special characters, URLs, and stop words. Applied tokenization and lemmatization.
2. **Vectorization**: Converted text data into numerical form using techniques like TF-IDF.

### Modeling
- **Baseline Model**: Built a logistic regression model to establish a baseline performance.

### Model Evaluation
- Used accuracy, precision, recall, and F1-score to evaluate model performance.
- Applied cross-validation to ensure the robustness of the models.

## Results
The best model achieved an accuracy of **87%** on the validation set. 


## Submission
The final predictions were saved in `submission.csv` and submitted to Kaggle for evaluation.

## Reproducing the Results
To reproduce the results, follow these steps:


