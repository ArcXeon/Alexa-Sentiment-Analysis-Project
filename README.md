# Alexa-Sentiment-Analysis
This is a project on performing Sentiment Analysis on Amazon Alexa Reviews using NLP.  
The working of the code is explained as follows:  
  
1.Data Loading and Exploration: The code starts by loading the data from a CSV file into a Pandas DataFrame. It then checks for null values and prints the value counts for the rating, variation, and feedback columns. It also generates countplots for these columns using the Seaborn library.  
  
2.Data Processing: The code defines a function data_processing that takes in a text string and performs several preprocessing steps, including converting the text to lowercase, removing URLs and punctuation, tokenizing the text into words, and removing stopwords. The code defines a function stemming that takes in a list of words and applies stemming to each word using the PorterStemmer from the NLTK library. This function is then applied to the verified_reviews column of the DataFrame.
  
3.Wordcloud Visualization: The code generates wordclouds for positive and negative reviews using the WordCloud library.It concatenates all of the verified_reviews into a single string, and generates a wordcloud from this string.  
  
4.Model Training and Evaluation: The code splits the data into training and test sets, with the verified_reviews column as the features (x) and the feedback column as the target (y). It uses a CountVectorizer to transform the text data into numerical data, which is then used to train a random forest classifier from the scikit-learn library. The trained model is used to make predictions on the test set, and the accuracy score, confusion matrix, and classification report are evaluated.  
