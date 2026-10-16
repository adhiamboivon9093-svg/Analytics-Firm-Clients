# Amazon Customer Reviews: 

# NLP Sentiment Analysis

1. Project Overview

This project uses Natural Language Processing (NLP) to analyse 997 Amazon customer reviews, understand customer opinions, identify common issues, classify sentiment, and flag negative reviews for follow-up.

2. What I Did

Explored the dataset and checked data quality.

Cleaned review text and applied tokenization, stopword removal, and lemmatization while preserving negation.

Identified common words, phrases, and customer concerns.

Compared Logistic Regression, Naive Bayes, DistilBERT, and a soft-voting ensemble.

Grouped reviews into topics and flagged negative feedback.

3. Key Results

77% of reviews were positive.

DistilBERT performed best, achieving 86% accuracy and a macro-F1 score of 0.541.

Accessories received the most reviews (291).

Customer Service / Returns had the highest negative-review rate (49.1%).

Negative reviews were flagged for further investigation.

4. Recommendations

Investigate customer service complaints, improve the detection of negative and neutral reviews, refine topic classification, and test the system on new data.

# Conclusion

The project demonstrates how NLP can classify customer sentiment, identify common concerns, and help businesses prioritize customer feedback. Further testing and human review are needed before using the system for real-world decisions.



# 2. Time Series Forecasting

1. Project Goal

Forecast monthly Amazon review activity to support customer support planning, review moderation, and resource allocation.

2. What I Did

Explored monthly review counts and average ratings.

Tested stationarity and seasonality using statistical tests and plots.

Compared Naïve, ARIMA, Exponential Smoothing, and SARIMA models.

Evaluated forecasts using MAE, RMSE, and forecast bias.

Forecast review activity for the next 12 months.

3. Key Results

The Naïve baseline performed best alongside ARIMA, achieving an MAE of 6.33 reviews and an RMSE of 7.90. The Naïve model was selected because it was simpler and equally accurate. Forecasts suggested approximately 15 reviews per month, although uncertainty increased over time.

# Conclusion

The project showed that time series forecasting can support operational planning. However, limited historical data and fluctuating review volumes mean forecasts should be treated as estimates and updated regularly as new data becomes available.

# 3. Neural Network Models

1. Business Goal

Build and compare machine learning models to classify Amazon reviews into 1–5 star ratings and predict numeric ratings.

2. What I Did

Inspected and cleaned 997 reviews.

Converted review text into numerical features using TF-IDF.

Built and evaluated Keras and PyTorch neural networks.

Compared classification models with Logistic Regression, Linear SVM, and simple baselines.

Built a neural network to predict numeric ratings.

3. Key Results

Logistic Regression: Best balanced classification performance, with a macro-F1 score of 0.340.

Keras classifier: Achieved 54.5% accuracy and a macro-F1 score of 0.338.

Linear SVM: Achieved 56% accuracy.

Keras regression: Achieved an MAE of 0.846, outperforming the mean-rating baseline.

# Conclusion

The project partially achieved its goal. Logistic Regression performed slightly better at balancing predictions across rating categories, while the regression model outperformed its baseline. However, models struggled with less common ratings. More data and improved text processing are needed before using these models for reliable business decisions.
