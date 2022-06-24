# Sarcasm Detector


![](https://images.fineartamerica.com/images/artworkimages/mediumlarge/3/funny-sarcasm-humor-provocative-sarcastic-gift-muc-designs.jpg)


#### -- Project Status: [Completed]

## Project Intro/Objective
The purpose of this project is to build an AI-powered system to be able to detect Sarcasm or Fake News from text content, to be more specific news headlines.

### Methods Used
* Deep Learning
* NLP
* Word2Vec
* RNN-LSTM

### Technologies
* Python
* Pandas, google colab

### The dataset
News Headlines dataset for Sarcasm Detection is collected from two news websites. 
* TheOnion: sarcastic versions of current events.  
* HuffPost: real (and non-sarcastic) news headlines.

Each record consists of three attributes:
    is_sarcastic: 1 if the record is sarcastic otherwise 0
    headline: the headline of the news article
    article_link: link to the original news article. Useful in collecting supplementary data

## Word2Vec
Word2Vec is an algorithm designed by Google that converts a word into vectors such that it groups similar words together into vector space. 
Usage examples: document retrieval, machine translation systems, autocompletion and prediction etc. 
In this notebook, I trained a Word2Vec model using the Gensim library.

source: https://www.askpython.com/python-modules/gensim-word2vec

## RNN-LSTM
Long Short Term Memory Network is an advanced RNN, that allows information to persist. It is capable of handling the vanishing gradient problem faced by RNN which is also used for persistent memory.
RNNs remember the previous information and use it for processing the current input. The shortcoming of RNN is, they can not remember Long term dependencies due to vanishing gradient. LSTMs are explicitly designed to avoid long-term dependency problems.

sources: https://www.analyticsvidhya.com/blog/2021/03/introduction-to-long-short-term-memory-lstm/

## FastText Embeddings
An extention of Word2Vec algorithm. FastText embeddings exploit subword information to construct word embeddings. Representations are learnt of character -grams, and words represented as the sum of the -gram vectors. This extends the word2vec type models with subword information. This helps the embeddings understand suffixes and prefixes. Once a word is represented using character -grams, a skipgram model is trained to learn the embeddings.

Source: https://paperswithcode.com/method/fasttext

## BERT and DistilBERT
A small, fast, cheap and light Transformer model based on the BERT architecture. The BERT transformer is a based deep learning technique for natural language processing (NLP) pre-training developed by Google on the entire Wikipedia dataset. BERT stands for Bidirectional Encoder Representations from Transformers.

source: https://arxiv.org/abs/1910.01108 
        https://arxiv.org/pdf/1810.04805.pdf
