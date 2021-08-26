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


