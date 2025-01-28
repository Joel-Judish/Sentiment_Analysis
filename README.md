# Sentiment Analysis Using NLTK

  This project demonstrates a simple sentiment analysis application using Python and the Natural Language Toolkit (NLTK). The application utilizes NLTK's SentimentIntensityAnalyzer from the VADER (Valence Aware Dictionary and sEntiment Reasoner) lexicon to evaluate the sentiment of an input text.

## Features
. Accepts user input as text.

Analyzes the sentiment of the input text.

Provides sentiment scores for the following categories:

Positive: Score representing positive sentiment in the text.

Negative: Score representing negative sentiment in the text.

Neutral: Score representing neutral sentiment in the text.

Compound: A normalized score ranging from -1 (most negative) to +1 (most positive).

Outputs the overall sentiment of the text as Positive, Negative, or Neutral.

Requirements

This project requires Python and the following libraries:

nltk: Install via pip (pip install nltk).

Installation

Clone this repository or download the script.

Install the required library by running:

pip install nltk

Download the VADER lexicon using the following Python code:

import nltk
nltk.download('vader_lexicon')

Usage

Run the script using a Python interpreter.

Enter a sentence when prompted.

The program will display:

Input text

Sentiment scores (positive, negative, neutral, compound)

The overall sentiment (Positive, Negative, or Neutral)

Example:

Enter a sentence to analyze sentiment: I love programming in Python!
Input Text: I love programming in Python!
Sentiment Scores: {'neg': 0.0, 'neu': 0.292, 'pos': 0.708, 'compound': 0.7783}
Overall Sentiment: Positive

Code Explanation

Library Import:

The nltk library is imported for sentiment analysis.

The SentimentIntensityAnalyzer class from nltk.sentiment.vader is used.

Download Resources:

The VADER lexicon is downloaded using nltk.download('vader_lexicon').

Sentiment Analysis Function:

The analyze_sentiment() function accepts a text input, computes sentiment scores, and evaluates the overall sentiment based on the compound score.

Compound score thresholds:

Positive: compound >= 0.05

Negative: compound <= -0.05

Neutral: otherwise

User Input:

The program takes user input via input() and passes it to the analyze_sentiment() function for analysis.

References

NLTK Documentation

VADER Sentiment Analysis

License

This project is licensed under the MIT License. See the LICENSE file for details.

