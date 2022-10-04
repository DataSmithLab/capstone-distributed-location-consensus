---
layout: page
title: "Decentralized Location Consensus"
doodle: "/doodle.png"
permalink: /
---

Data science capstone domain of inquiry (DSC 180A B16)

Developed by Haojian Jin.

---
* TOC
{:toc}

---

# Introduction

Many features in mobile apps rely on authentic smartphone location data. For example, Pokemon Go uses location to track players’ movement; dating apps use location to match people. However, it is surprisingly easy to spoof the location by hacking the OS, Radio, and mobile Apps. In this project, we will explore and design new mechanisms to create a decentralized location consensus, where participants can prove to the world that their phones have been to a specific location. 


This domain of inquiry seeks to design computing systems that can generate privacy-sensitive location proofs.
To approach this problem, we will initially focus on studying a secure, decentralized, privacy-preserving proximity tracing system, named [DP3T (Decentralized Privacy-Preserving Proximity Tracing)](https://github.com/DP-3T/documents). We will then retrofit this tool into a system that can generate privacy-sensitive location proofs in the future. 



## Result replication (introduction to topic)

We will first setup the DP3T and study how they implement the programs:
* [Android demo](https://github.com/DP-3T/dp3t-app-android-demo)
* [dp3t-sdk-android](https://github.com/DP-3T/dp3t-sdk-android)
* [dp3t-sdk-backend](https://github.com/DP-3T/dp3t-sdk-backend)


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
|1|[Introduction to Decentralized Location Consensus and DP3T]({{ "weeks/01-Introduction" | absolute_url }})|
|2|[Code: Deploy the end-to-end demo]({{ "/weeks/02-Source-Code" | absolute_url }})|
|3| Bluetooth low energy signal calibration |
|10|Present Proposals|

<!-- |3|[Creating Graphs from Code; What is Malware?]({{ "/weeks/03-Android-Graphs" | absolute_url }})| -->
<!-- |4|[Graph Invariants as Measurements]({{ "/weeks/04-Graph-Features" | absolute_url }})| -->
<!-- |5|[Building a Baseline Model]({{ "/weeks/05-Baseline-Model" | absolute_url }})| -->
<!-- |6|[Evalulating the HinDroid Result]({{ "/weeks/06-Hindroid" | absolute_url }})| -->
<!-- |7|[Graph Embedding I: node2vec]({{ "/weeks/07-Graph-Embeddings-I" | absolute_url }})| -->
<!-- |8|[Graph Embedding II: metapath2vec]({{ "/weeks/08-Graph-Embeddings-II" | absolute_url }})| -->
<!-- |9|[Production and Adversarial ML]({{ "/weeks/09-Adversarial-ML" | absolute_url }})| -->

---

# Discussion hours

Monday 4-5PM, SDSC 



