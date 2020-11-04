---
layout: week
title: Week 01
permalink: /weeks/06-Hindroid/
doodle: /doodle.png
---

# Week 6: Evalulating the HinDroid Result

NOTE: Due to the Wednesday holiday, this week we will be meeting
Friday at 9AM PST.


## Topics

This week's assignments will guide you through the following topics:
* Review SVMs and the kernal trick.
* Implement the basic Hindroid Malware Classifier.
* Assess different choices of kernel.

## Reading

Please read the following:
* Hindroid sections 3 and 4, paying particular
  attention to the table of results evaluating the different
  metapaths.
* Review
  [this](https://monkeylearn.com/blog/introduction-to-support-vector-machines-svm/)
  tutorial. It is a succinct 5-min read that should help your revise
  SVM. Assume red-triangles are malwares and blue-circles are benign
  apps.
* For more review on SVMs,
  [this](https://www.youtube.com/watch?v=_PwhiWxHK8o) is really a
  great lecture and these are some great
  [slides](http://web.mit.edu/6.034/wwwbob/svm-notes-long-08.pdf).
  
## Tasks

Complete the following tasks:
* Develop code that can calculate the commuting matrices formed by
  products of `A`, `B`, `P`. (Refer to week 05 for a hint on sparse
  matrices!)
* Implement the Hindroid Malware classifier for various kernels on a
  dataset from DSMLP.Try training models with kernels: `AA^T`,
  `ABA^T`, APA^T`, `APBP^TA^T`. See implementation note below.
* Evaluate the performance of the above classifiers on different
  Malware types. (How are you splitting train and test?)

### Note on Implementation

Hindroid's model is an SVM classifier with a custom kernel. Recall
that SVMs only need the dot-product of the data-points for
classification, in our case, this will be the commuting matrix
*M*<sub>*p*</sub>[*i*][*j*], where *i* and *j* are the indexes
corresponding to the Apps.

You can use scikit's [SVM](https://scikit-learn.org/stable/modules/svm.html)
for your assignment. As explained above you are going to assume that
you already have the pre-computed kernel matrix in the form of
*M*<sub>*p*</sub>. Hence, you will need to use [custom
kernels](https://scikit-learn.org/stable/modules/svm.html#custom-kernels).

More specifically, you can directly use
[Gram-Matrix](https://scikit-learn.org/stable/modules/svm.html#using-the-gram-matrix).


## Weekly Questions

Answer the following questions on Canvas:

* What properties do these different meta-paths capture in the data?
* Why do all of the meta-paths in the Hindroid kernels start and end
  with the adjacency matrix A?
* Use the test data to train a classifier with kernel `ABA^T` and
  compute the resulting f1-score.
  


