---
layout: week
title: Week 01
permalink: /weeks/08-Graph-Embeddings-II/
doodle: /doodle.png
---

# Graph Embedding II: metapath2vec

## Topics

Now we know about *word2vec* and *node2vec*. We also understand why we can't directly apply *node2vec* on HinDroid. This week we are going to study metapath2vec which will address this shortcoming.

## Reading

### metapath2vec
Pls go through the [paper](https://ericdongyx.github.io/papers/KDD17-dong-chawla-swami-metapath2vec.pdf) thoroughly. We are going to majorly focus on this paper next Wednesday.

The gist of the paper is that we choose the *type* of metapath to traverse to generate a neighbourhood. By doing so we don't let a specific edge type dominate the rest while generating the neighbourhood.


## Task
Consider the following graph:

<img src="https://raw.githubusercontent.com/afraenkel/capstone-malware-domain/master/images/metapath2vec.png" alt="Graph" class="inline" width="400"/>

At, 

t=0, node = S\
t=1, node = a

Landing Nodes:\
A. Green (I)\
B. Red (B)\
C. Yellow (P)

Q1. If we are following node2vec then at t=2, what is the probability of landing on the above nodes for the following three cases:

<img src="https://raw.githubusercontent.com/afraenkel/capstone-malware-domain/master/images/node2vec.png" alt="" class="inline" width="200"/>


Q2. If we are following metapath2vec, then at t=2, what is the probability of landing on the above nodes for the following three cases:

<img src="https://raw.githubusercontent.com/afraenkel/capstone-malware-domain/master/images/mp2vec.png" alt="" class="inline" width="300"/>


## Weekly Questions

* From the metapath2vec paper, provide any 3 sentences from the first three sections (Intruduction, Problem Statement and the Framework) that you think cogently explains the problem statement and the approach.
* Last week we learned about node2vec. Why can't we directly use node2vec to solve our problem (we discussed this on Wednesday)?
* Do you think metapath2vec can address this problem? Explain briefly.