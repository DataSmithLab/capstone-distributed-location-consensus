---
layout: week
title: Week 01
permalink: /weeks/06-Hindroid/
doodle: /doodle.png
---

# Week 6: Evalulating the HinDroid Result

## Topics

This week's assignments will guide you through the following topics:
* Implement the basic Hindroid Malware Classifier.
* Assess different choices of kernel.

## Reading

Please read the following:
* Hindroid sections 3 and 4, paying particular
  attention to the table of results evaluating the different
  metapaths. 
* reading 2

## Tasks

Complete the following tasks:
* Implement the Hindroid Malware classifier for various kernels on a
  dataset of your design. (Try kernels: `AA^T`, `ABA^T`, APA^T`,
  `APBP^TA^T`).
* Evaluate the performance of the above classifiers on different
  Malware types.

## Weekly Questions

Answer the following questions on Canvas:

* What properties do these different meta-paths capturing in the data?
* Why do all of the meta-paths in the Hindroid kernels start and end
  with the adjacency matrix A? (*)
* Which kernels do best at classfying which types of Malware?
* A dataset will be placed in `/datasets/dsc180awi20/Malware/test`
  with subdirectories `positive` and `negative`. Use this data to
  train a classifier with kernel `ABA^T` and compute the resulting
  accuracy. (*)
  


