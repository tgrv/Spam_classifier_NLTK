# Spam Mail classifier using NLTK

This notebook contains a Spam Mail classifier built using NLTK's Naive Bayes claasifier. The dataset can be obtained from the following link:
http://s3.amazonaws.com/istreet-assets/YvuOzNGw5MCDwRwOcljf3g/emails.csv

Steps performed:

1. Load the dataset.
2. Since there is a class imbalance, we will stratify while splitting into train and test sets.
3. Tokenize input text (including lemmatizing, lower-casing, removing stopwords).
4. Create feature vectors for each input mail, based on vocabulary consisting of 2000 most commonly occuring words (from training set).
5. Train Naive Bayes classifier with feature vectors and corresponding labels.
6. Predict our test data, and check accuracy