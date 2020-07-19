**Lesson 2: Intro to Machine Learning**

# Chapter 11 - Text Data
*Tokenizing* text is spliting each string of text into a list of smaller parts or tokens
## Normalization

> Text normalization is the process of transforming a piece of text into a canonical (official) form.

### Lemmatization
A lemma is the dictionary form of a word and lemmatization is the process of reducing multiple inflections to that single dictionary form.


**Examples:** 

Original word |	Lemmatized word
---------|----------
is | be
are|	be
am	| be
## Stop words removal
>  Stop words are high-frequency words that are unnecessary (or unwanted) during the analysis. 

**Examples:** 

Original text|  Normalized text
---------|----------
The quick fox.	| [quick, fox]
The lazzy dog.	| [lazy, dog]
The rabid hare.| 	[rabid, hare]
Most have small cardinality eg Gender. Some have high eg Location ID

## Vectorization
After normalization, the next step is usually vectorization- encoding it into a numerical form.
### Common approaches
* Term Frequency-Inverse Document Frequency (TF-IDF) vectorization: Assigns weights to words that signify their relevance in the documents.
* Word embedding, as done with Word2vec or Global Vectors (GloVe)

## Feature Extraction

## The whole pipeline
1. Normalize
2. Vectorize and Extract Features
3. Train model
4. Deploy model