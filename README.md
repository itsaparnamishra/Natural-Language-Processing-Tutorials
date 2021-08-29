# Natural-Language-Processing-Tutorials
Getting started with NLP (Basics)


# What is Tokenization ? 
Tokenization is converting paragraphs into list of words and sentences. In order to get our computer to understand text we use tokenization which is basically the breakdown of texts into words,sentences and subwords. Tokenization plays a significant role in dealing with text data.
	
Tokenization is a way of separating a piece of text into smaller units called tokens. 


# What is Stemming ?
Stemming is a technique which is used in NLP to extract the stem word from a branch of words, for example : pull, pulls, pulling, pulled has a stem word "pull".
Some of the stemming algorithms are PorterStemmer,Lancaster Stemming Algorithm, RegexpStemmer ,Snowball stemming algorithm.


# What is Lemmatization ?

from nltk.stem import WordNetLemmatizer----> NLTK provides WordNetLemmatizer class for lemmatization.
Lemmatization is used for stemming unlike PorterStemmer class , Lemmatization technique using WordNetlemmatizer class returns meaningful root words.

# Difference between Stemming and lemmatization :

The PorterStemmer class gives words which are not meaningful although it is also used for stemming, but WordNetLemmatizer class returns meaningful root words.
So, we can conclude that Lemmatization technique always gives valid words unlike Stemming technique.

# Bag of Words (BoW)

Bag of Words is used to convert text data/corpus into meaningful numerical data in the form of an array so that it can be further used in building NLP model.
It basically represents words into numbers so that the model can process it. This step is taken care by CountVectorizer method which is present in sklearn.feature_extraction.text (from sklearn.feature_extraction.text import CountVectorizer) , but before converting the text data into numerical data we need to clean the corpus , all the methods are shown in the jupyter notebook - NLP BagOfWords.

Drawbacks of BoW :
1) It only gives how many times a word occurred in a sentence and not its location or correlation with other words.
2) It gives equal importance to all the words in the sentence.
3) Other methods like TFIDF and word2Vec are used instead of BoW.


# TF-IDF : Term frequency Inverse Document Frequency 
It is used to define how relevant a word in a corpus is to other words. Better than BoW.

1) Formula to find TF = [ (no. of repetition of word in the sentence) / (no. of words in the sentence) ]
2) Forumula to find IDF = log [(no. of sentences) / (no. of sentences containing the words) ]
3) TF-IDF = TF * IDF 

This step can be implemented by Tfidfvectorizer method after cleaning the corpus.
The NLP TF-IDF notebook contains all the steps explaining TF-IDF


# SMS Spam Classifier 
Used TF-IDF model, Naive Bayes Classifier from sklearn.naive_bayes, confusion matrix from sklearn.metrics for matching y_test and y_pred , lastly used accuracy score from sklearn.metrics to check the accuracy which came out to be 97%. The SMS Spam Classifier notebook includes all the steps.
The data was extracted from https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection 




