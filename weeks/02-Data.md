---
layout: week
title: Week 02
permalink: /weeks/02-Data/
doodle: /doodle.png
---

# Data: Code Parsing, Malware

## Topics

This week's assignments will guide you through the following topics:
* What is Malware? What does it do?
* Identifying Malware by code structure: Libraries, APIs, and network
  calls.
* Disassembling Android bytecode to Smali code (and interpreting it).


## Reading

Please read the following:
* **Hindroid Section XX**
* Read
  [slides](http://www.syssec-project.eu/m/page-media/158/syssec-summer-school-Android-Code-Injection.pdf)
  on the process of creating Smali code. The slides more generally
  speak about recompiling an App after changing Smali code (perhaps
  injecting malicious code). While interesting, you only need to focus
  on the slides decribing the correspondence between Java source code
  and Smali code. [This](http://pages.cpsc.ucalgary.ca/~joel.reardon/mobile/smali-cheat.pdf) 
  is also a very handy guide for quick access to smali syntax.
* Read this
  [post](https://duo.com/decipher/hunting-malicious-npm-packages)
  about searching for malicious Javascript using static code
  analysis. This article uses the dependency graph of different
  programs to emphasize how much unknown code you may be installing,
  even when installing a "trusted" library (`npm` is javascripts package
  manager, much like python's `pip`).


## Tasks

Complete the following tasks:

**Apks and Smali Code**

Android apps are written in Java and compiled to *Dalvik* bytecode,
and distributed in zipped files called *apk*s, to be run on a
phone. The bytecode is denoted with the `.dex` file suffix. To
statically analyze android code, we need to decompile these `dex`
files to a representation in what's called *Smali code*. Since we will
be attempting to understand what code does from Smali files, we need
to understand how Smali represents Java source code.

1. To download `apk` files directly on your computer, you can use
   [www.apkpure.com](https://www.apkpure.com). To obtain an apk file from the
   play store, you would need to install it on a phone, then grab the
   file from the mobile device (not recommended).
2. To decompile an Android Apk to Smali code, download and use
   [ApkTool](https://ibotpeaches.github.io/Apktool/). Follow the
   download instructions and run it on a sample (benign) android app.

**Measurements from Code**

* Calculate stats on a single apk.
* Reason through what you *think* stats might be for Malware
* Bonus: Calculate stats on many apks


## Weekly Questions

Answer the following questions on Canvas:
* What are the components of Smali?
* ...
* What are private classes?
