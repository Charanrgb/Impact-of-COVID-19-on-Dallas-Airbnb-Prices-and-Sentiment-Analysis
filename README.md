# Impact-of-COVID-19-on-Dallas-Airbnb-Prices-and-Sentiment-Analysis


Overview

This project explores the impact of the COVID-19 pandemic on Dallas Airbnb listings, focusing on price trends, booking patterns, and guest sentiments. Using data-driven techniques such as Random Forest, Linear Regression, and sentiment analysis models (RoBERTa, BERT, VADER), we analyzed changes before and after the pandemic to understand market recovery and key influencing factors.

Objectives

Analyze price trends and booking patterns before and after the COVID-19 pandemic.

Identify changes in user preferences (e.g., property type) during the pandemic.

Perform sentiment analysis on Airbnb reviews to detect trends in guest satisfaction.

Evaluate and compare the effectiveness of sentiment analysis models.

Dataset

Source: Dallas Airbnb dataset

Size: 132,975 reviews (2016–2024)

Features: Review text, ratings, room type, host attributes, etc.

Preprocessing:

Handling missing values.

Feature reduction.

Categorical conversion.

Research Questions

How did the COVID-19 pandemic impact Airbnb pricing, bookings, and availability in Dallas?

Are there significant changes in user preferences (e.g., property type) before and after COVID-19?

What are the most common sentiments expressed in reviews for Dallas Airbnbs?

What is the best model (RoBERTa, BERT, or VADER) for sentiment analysis?

Methods and Models

Data Processing

Divided data into pre-COVID (2016–2020) and post-COVID (2020–2024).

Target variable: price.

Selected key features: price, bedrooms, bathrooms, accommodates.

Descriptive Statistics

Used correlation heatmaps to identify important features.

Pricing Analysis

Linear Regression

Before COVID (2016–2020):

Adjusted R²: 0.94

MSE: 330.33

RMSE: 18.17

After COVID (2020–2024):

Adjusted R²: 0.0272

MSE: 205789.21

RMSE: 453.64

Random Forest

Before COVID (2016–2020):

R²: 0.94

MSE: 343.12

RMSE: 18.52

After COVID (2020–2024):

R²: 0.05

MSE: 201042.26

RMSE: 448.38

Sentiment Analysis

Evaluated models: RoBERTa, BERT, VADER.

Focused on reviews from the last year for computational efficiency.

Model Comparisons

RoBERTa:

Average Score: 0.873

Highlights strong positivity in reviews.

BERT:

Average Score: 0.865

Displays similar results but slightly less effective.

VADER:

Average Score: 0.759

Rule-based model with limited context understanding.

Key Findings

Pre-COVID, both Linear Regression and Random Forest performed well (R² ≈ 0.94).

Post-COVID, performance dropped significantly due to market volatility.

RoBERTa outperformed other sentiment models due to its ability to capture nuanced sentiment.

Reviews are overwhelmingly positive, with minimal negative outliers.

Conclusion

RoBERTa is the best sentiment analysis model for this project due to its accuracy and ability to detect positive sentiment.

The COVID-19 pandemic significantly impacted Airbnb pricing and booking patterns in Dallas, with predictive models struggling to adapt to post-COVID trends.

Technologies Used

Programming Language: Python

Libraries:

Data Analysis: pandas, numpy

Visualization: matplotlib, seaborn

Machine Learning: scikit-learn

Sentiment Analysis: transformers (Hugging Face), nltk



