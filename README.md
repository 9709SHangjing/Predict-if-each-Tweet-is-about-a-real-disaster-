# Predict-if-each-Tweet-is-about-a-real-disaster-
Predict if each Tweet is about a real disaster through NLP
1. In this problem, I will implement several machine learning
techniques to perform classification on text data. Throughout the problem, I
will be working on the NLP with Disaster Tweets Kaggle competition, where the task is to predict
whether or not a tweet is about a real disaster.

2. Some steps performed in this project are as follow:
   * Data cleaning and filtration - Basic Statistical analysis
   * Split the training data: Since we do not know the correct values of labels in the test data,
     we will split the training data from Kaggle into a training set and a development set (a development
     set is a held out subset of the labeled data that we set aside in order to fine-tune
     models, before evaluating the best model(s) on the test data). Randomly choose 70% of the
     data points in the training data as the training set, and the remaining 30% of the data as the
     development set. Throughout
   * Preprocess the data:
      1. Convert all words to lowercase
      2. Lemmatize all the words
      3. Strip punctuation
      4. Strip the stop words, e.g., “the”, “and”, “or”
      5. Strip @ and urls. (It’s Twitter.)
   * Bag of Words Model: extract features in order to represent each tweet using
     the binary “bag of words” model, as discussed in lectures. The idea is to build a vocabulary
     of the words appearing in the dataset, and then to represent each tweet by a feature vector
     x whose length is the same as the size of the vocabulary, where xi = 1 if the i ’th vocabulary
     word appears in that tweet, and xi = 0 otherwise.
   * Perform Logistics Regression and evaluate the model based on the F-1 score 
   * Implement a Bernoulli Naive Bayes classifier and evaluate the F-1 score 
   * Compare Naive Bayes model and Logistics Regression Model 
