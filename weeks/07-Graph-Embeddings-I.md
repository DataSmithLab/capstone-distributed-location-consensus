---
layout: week
title: Week 01
permalink: /weeks/07-Graph-Embeddings-I/
doodle: /doodle.png
---

# Graph Embedding I: node2vec

## Introduction

We have used the graph that we constructed on the Android Apps to build a SVM based classifier.
Now, can we use deep-learning based approaches instead?
Most of the deep learning approaches require features as input. As we saw, SVM uses the kernel trick to learn the classifier without explicitly learning the features for the nodes. So, how do we learn features from this graph?

This and the next week we will learn about a techinique called [metapath2vec](https://ericdongyx.github.io/papers/KDD17-dong-chawla-swami-metapath2vec.pdf) that learns a distributed representation of nodes based on its connections. But to understand metapath2vec, we first need to understand the following:

## word2vec - Representing words with vectors

[Word2Vec](https://arxiv.org/pdf/1301.3781.pdf) was published in 2013 in which Mikolov et al. suggest a method to learn distributed representations of words based on the **context** in which it appears. The problem they is trying to solve is finding features for words. They build upon the [distributional hypothesis](https://en.wikipedia.org/wiki/Distributional_semantics) which suggests that 'words that are used and occur in the same contexts tend to purport similar meanings'. They propose two methods to do the same. 1) CBOW - Continuous Bag of Words and 2) Skip-gram. I highly recommend reading [word2vec-Explained](https://arxiv.org/pdf/1402.3722.pdf) paper *before* going through the actual [word2vec](https://arxiv.org/pdf/1301.3781.pdf) paper. [This](https://arxiv.org/pdf/1310.4546.pdf) is an extension of word2vec.

If you want to get a feel of what word2vec are or how to use them, this is a very good [resource](https://gist.github.com/aparrish/2f562e3737544cf29aaf1af30362f469).

## node2vec

Building on the work of word2vec, [node2vec](https://arxiv.org/pdf/1607.00653.pdf) proposed a method to learn distributed representation for the nodes in a (homogenous) network. They propose a biased random walk procedure to explore the network and learn the embeddings using the same. You can refer [DeepWalk](https://arxiv.org/pdf/1403.6652.pdf) if you find node2vec abstruse as it builds upon DeepWalk.

## Readings
Please go through [The illustrated word2vec](http://jalammar.github.io/illustrated-word2vec/), [word2vec-Explained](https://arxiv.org/pdf/1402.3722.pdf) and [node2vec](https://arxiv.org/pdf/1607.00653.pdf) prior to this week's discussion. It is completely fine if you don't understand them completely but please try to understand the problem they are trying to solve.

## Links
[The Illustrated Word2vec](http://jalammar.github.io/illustrated-word2vec/)\
[Skip-Gram tutorial](http://mccormickml.com/2016/04/19/word2vec-tutorial-the-skip-gram-model)\
[Word2Vec](https://arxiv.org/pdf/1301.3781.pdf)\
[Word2Vec's extension](https://papers.nips.cc/paper/5021-distributed-representations-of-words-and-phrases-and-their-compositionality.pdf)\
[Word2Vec Explained](https://arxiv.org/pdf/1402.3722.pdf)\
[DeepWalk](https://arxiv.org/pdf/1403.6652.pdf)\
[node2vec](https://arxiv.org/pdf/1607.00653.pdf)\
[node2vec tutorial](https://towardsdatascience.com/node2vec-embeddings-for-graph-data-32a866340fef)

## Weekly Questions

Answer the following questions on Canvas:

Q1. What are the two different model architectures proposed in Word2Vec paper? Explain what they are trying to do in one line each.

Q2. Can we directly apply node2vec to the graphs that we have built? If yes, how do you extract the features? If no, why not? 

Q3. What could be the benefits of n2v based method over HinDoird?

Implementation: (Shouldn't take more than 10 lines of code and 15 mins)

Q4. Use gensim library to train (use default config) a w2v model on brown corpus and answer the following questions. Follow [this](https://medium.com/@mishra.thedeepak/word2vec-in-minutes-gensim-nlp-python-6940f4e00980) tutorial.

A) First 10-dimensions of the representation of the following words: book, king, queen, sun.

B) List top 5 most similar words of the following: book, king, queen, sun. (Use model.most_similar method)