# Tweets_keyphrase_extraction
This aims to study Key Phrase extraction using Deep Recurrent Neural Network.

I have tried to develop on the work and learnings from the research paper - 
Key Phrase Extraction using
Deep Recurrent Neural Network on Twitter Qi Zhang, Yang Wang,
Yeyun Gong, Xuanjing Huang - 2016, Association for Computational
Linguistics
https://github.com/fudannlp16/KeyPhrase-Extraction

The joint layer concept comes from the need of doing joint processing of 2 sub-objectives, which will be combined into the main objective function.
Computing one feature and passing it to other, will cause the error to propagate into further layers.
**Hence, this model is a 2-layer joint recurrent neural network.**

The aim of layer 1 is to detect whether the input word at instance t, is a keyword or not. 

Layer 2 focuses on keyword extraction. It assigns a label to the word that tells at what part the word would occur in a key-phrase.

# Input data
The neural network was fed with
Word Embeddings as input. Word embedding represents document vocabulary. It captures context of a word in a document, semantic and syntactic
similarity, relation with other words, etc.

