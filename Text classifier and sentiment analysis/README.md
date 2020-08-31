![](C:\Users\danie\Desktop\presentacion ironhack\logo.svg)

# Text classifier for Spanish text

César Campuzano

Data Analytics bootcamp final project.

## Overview

The main idea for this project was to perform a sentiment analysis of the main banking institutions in Mexico, by scrapping social media, specifically Twitter.  Nevertheless, through the process I realized that those NLP python libraries out there such as NLTK, Spacy or Textblob  were not made to classify the polarity  of any given text. Reason why I challenged myself to create a model through ML which can classify a text in either positive or negative, better known as sentiment analyzer.

## Data

I have to thank the people from SEPLN.org which were kind enough to provide me with a dataset, better known as Corpus, consisting of over 1800 tweets in Spanish language (Mexican) which was previously labeled by them (a task they perform and update every single year). 

The data was preprocessed through the following steps:

- [ ] Cleaning .- Which involved removing any symbols and numbers.

- [ ] Tokenizing.- Which consists in splitting the words of the tweet to be analyzed independently.

- [ ] Stop-words.- Words that don't provide any special value such as 'the', 'my', with, are, etc., were removed.

- [ ]  Lemmatizing.- Which converts words to its given root without losing the it's meaning in contrast with Stemming which reduces the word to its root but not considering the meaning of it. This makes it easier for the computer to understand the meaning of different words that have the same meaning., e.g.,

  ​				'running'- 'run'

  ​				'eating' - eat

  ​				'threw' - 'throw'

- [ ] Vectorizing.- Which consists of creating a list of words with its corresponding frequency found within the dataset.

  

  

## Model

I used a Deep Learning model called Sequential found within keras's library which performs really good when it comes to binary classifications. 

With the data obtained in the corpus I created a vocabulary of the main words found within in order to predict the polarity of a given text.

At the moment the model is able to classify a text written in Spanish in either positive or negative with a 68% accuracy.

According to the experts in the NLP field a model with a 60% accuracy is considered good and a model which can achieve over a 70% accuracy is considered outstanding since it is proven that even us humans cannot agree on the polarity of a given text in 30% of the times. So achieving 70% accuracy for a computer is considered almost human, so to say.

The model was finally saved as a pickle file which you can find within the repo for your use.



## Conclusions

Achieving a 68% accuracy with the given data was good as a first approach to the topic, nevertheless, there is still a lot of room for improvement in the NLP field specifically when it comes to analyzing sentiment in Spanish language. Reason why I have a few next steps which I am planning to develop in the near future:

- [ ] Improve the accuracy performance of the model by feeding more data and exploring others.
- [ ] Train the model in order to detect sarcasm within a given text.
- [ ] Make the model public through a web page where with few knowledge about this topic can easily perform a sentiment analysis.



## Tools used

- [ ] Python
- [ ] Pandas
- [ ] Numpy
- [ ] Spacy
- [ ] NLTK
- [ ] Keras
- [ ] Tableau