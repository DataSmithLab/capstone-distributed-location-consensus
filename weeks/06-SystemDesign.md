---
layout: week
title: Week 01
permalink: /weeks/06-SystemDesign/
doodle: /doodle.png
---

# Week 6: System Design


## Topics

This week's assignments will guide you through the following topics:
* Read the source code with the white paper.
* Start to implement a minimum viable product.
* Think about the final design.

## Reading

Please read the following:
* Make sure you understand section 2.2 and 2.3 [DP3T whitepaper](https://github.com/DP-3T/documents/blob/master/DP3T%20White%20Paper.pdf). Now you are getting familiar with the codebase. So you can look at how they implement each piece of code. 
*  Make sure you understand section V. EXPERIMENTS AND RESULTS [Global attestation of location in mobile devices](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7357675). Think about how we should design/implement these pieces.
  

## Key questions

[Calibration app](https://github.com/DP-3T/dp3t-sdk-android) 
1. How does the phone generates a random message? 
2. How do the phones exchange messages?
3. How does the phone store messages locally? What message does the phone send to the server? 
4. How does the phone check if the user is exposed for a long enough time?


[dp3t-sdk-backend](https://github.com/DP-3T/dp3t-sdk-backend)
1. How does the server encrypt/decrypt users' data?
2. What data does the server return to the phones?
3. How does the server handle data from users who got CoVID-19?
4. What data would be stored on the server?

## Tasks

1. Assign each question to one team member. 
2. Locate the exact code fragment.
3. Write pseudo code to modify it into a minimum viable product prototype. 



### Note on Implementation

1. Suggest the Android team use ["prestandard" codebase](https://github.com/DP-3T/dp3t-sdk-android/releases/tag/prestandard). 
2. Download the source in that URL.
3. Commit the source code into a git repository. So you guys can work on the same repository. 
4. The main msg generation/communication files are BleServer.java and BLEClient.java. (Here is how you can search a file by file name in GitHub. https://stackoverflow.com/a/61471327 ) 
5. Suggest the server team build a backend from scratch using Django. 


## Weekly Questions

Answer the following questions on Canvas:

* Which question would you work on?
* Locate the source code for your question?
* Write pseudo code to describe your planned implementation? 
  


