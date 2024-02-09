Sentiment Analysis of Elon Musk's Tweets


Project Overview
This project involves the development of Natural Language Processing (NLP) models to analyze sentiment in tweets posted by Elon Musk. 
The goal is to gain insights into the sentiment of Elon Musk's tweets, particularly those related to Tesla and other topics of interest,
and to explore the potential relationship between sentiment and stock market movements. Various machine learning models, including linear regression, 
random forest regressor, and a Multi-Layer Perceptron (MLP) classifier, were trained and evaluated to predict sentiment scores based on tweet content.

Dataset
The dataset used in this project consists of a collection of Tesla stock prices during a specific period of time and  collection of tweets posted by Elon Musk over the 
same period of time, capturing his thoughts, announcements, and interactions related to Tesla and other topics of interest. 
Each tweet in the dataset includes information such as the tweet ID, tweet content, and the date and time it was posted. 
The dataset was obtained using the Twitter API, which allows access to public tweets based on specific search criteria.


Preprocessing
The preprocessing steps involved in this project aim to clean and prepare the tweet data for sentiment analysis and prediction of stock market movements. This includes:
Removal of special characters, punctuation marks, emojis, and symbols to reduce noise and focus on relevant text content.
Stop word removal by filtering out commonly used words that do not carry significant meaning in sentiment analysis.
Calculation of sentiment scores using the SentimentIntensityAnalyzer tool from the NLTK library, which assigns sentiment scores ranging from -1 to 1 based
on lexical and grammatical features.


Model Training and Evaluation
Linear Regression: Initial attempts with linear regression yielded a perplexing R-squared score of -1, suggesting poor performance in capturing the relationship 
between sentiment scores and stock market movements.
Random Forest Regressor: The evaluation of the random forest regressor model yielded an even worse R-squared score of -4, indicating significant difficulty in 
capturing underlying patterns in the data.
MLP Classifier: The Multi-Layer Perceptron (MLP) classifier showed promise by achieving a relatively better R-squared score of 0.23. 
This suggests that the MLP classifier was able to capture more of the underlying patterns in the sentiment scores and their relationship to stock market movements.

Model Optimization
Cross-Validation: Cross-validation was applied to improve the reliability and generalization of the MLP classifier's performance, resulting in a relatively lower 
accuracy compared to a single train-test split.
Ensemble Methods: Bagging was applied to the MLP classifier, but it did not significantly affect the accuracy of the model, 
indicating that the MLP classifier already performs well on its own and that the dataset is not very prone to overfitting.

Conclusion
In conclusion, initial attempts with linear regression and random forest regressor proved to be less effective in capturing the complexities of the data. 
However, the MLP classifier showed promise by achieving a relatively better performance. 
Further analysis and fine-tuning of the models, as well as consideration of additional factors and alternative models,
may be necessary to improve the accuracy of stock market prediction using sentiment scores derived from Elon Musk's tweets.
