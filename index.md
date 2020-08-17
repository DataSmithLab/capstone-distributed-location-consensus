---
layout: page
title: "Understanding Code Through Graphs"
doodle: "/doodle.png"
permalink: /
---

Data science capstone domain of inquiry (DSC 180AB A04)

---
* TOC
{:toc}

---

# Introduction

This domain of inquiry studies the problem of understanding computer
code through machine learning on graphs. To approach this problem, we
will initially focus on the problem of *malware detection* in Android
applications.

In this domain, project proposals will be restricted to the following
areas:
* Computer Code Understanding (using a variety of techniques)
* Data Driven Approaches to Malware and Cyber-Security

This domain centers around understanding computer code as *data*. You
will spend a significant amount of work writing parsing logic for this
code that measures the behaviors of interest (i.e. data processing).

## Result replication (introduction to topic)

The bulk of the first half of the project will focus the task of
"computer code understanding" on the specific problem of detection
whether given source code is Malware or a benign application. The bulk
of the result replication will focus on static code analysis using
machine learning on graphs, as developed in the following papers:
* [Hindroid](https://www.cse.ust.hk/~yqsong/papers/2017-KDD-HINDROID.pdf)
* [MaMaDroid](https://arxiv.org/pdf/1612.04433.pdf)

The latter-half of Quarter 1 will introduce you to further topics,
like graph embedding techniques and adversarial ML, to inform possible
avenues for further research.

## An initial note on ethics

The ability to identify and combat Malware requires understanding how
Malware works. Such knowledge is divorced from how it gets used by the
practitioner; you, as the practitioner must be aware of ethical
concerns with the usage of this knowledge and behave accordingly. In
particular, while working with the material in this course, you must
never engage in illegal activity related to your coursework and you
must adhere to the code of academic integrity, as laid out in th
syllabus.

The topic of ethics will be regularly approached in this domain. For
more reading on the ethics of teaching Malware, see this opinion
pience [On the Growing Harm of Not Teaching
Malware](http://www.csl.sri.com/users/neumann/cacm223.pdf) and a
related study on [the ethics of teaching
malware](https://www.ieee-security.org/TC/SPW2014/papers/5103a001.PDF).

---

# Section Participation

Participation in the weekly discussion section is *mandatory*. Each
week, you are responsible for doing the reading/task assigned in the
[schedule](#schedule). Come to section prepared to ask questions about
and discuss the results of these tasks.

Each week, turn in answers to the weekly questions to Canvas. These
questions are meant to focus your work for the week and help prepare
you for discussion. If you have questions about your work, please ask
them in section or office hours (I will rarely comment on your
submission).

You are responsible for the entire weekly reading/task, even if
portions are not covered in the weekly questions. The weekly tasks are
the building blocks for the project proposals/assignments due at the
end of the quarter.

---

# Schedule

|Week|Topic|
|--|--|
|1|[Introduction to Code-Understanding and Malware]({{/weeks/01-Introduction | absolute_url }})|
|2|[Data: Code Parsing, Malware](/weeks/02-Data)|
|3|[Creating Graphs from Code; What is Malware?](/weeks/03-Android-Graphs)|
|4|[Graph Invariants as Measurements](/weeks/04-Graph-Features)|
|5|[Building a Baseline Model](/weeks/05-Baseline-Model)|
|6|[Evalulating the HinDroid Result](/weeks/06-Hindroid)|
|7|[Graph Embedding I: node2vec](/weeks/07-Graph-Embeddings-I)|
|8|[Graph Embedding II: metapath2vec](/weeks/08-Graph-Embeddings-II)|
|9|[Production and Adversarial ML](/weeks/09-Adversarial-ML)|
|10|Present Proposals|

---

# Office Hours





