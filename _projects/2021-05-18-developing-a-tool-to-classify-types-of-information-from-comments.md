---
title: "Developing a Tool to Classify Types of Information from Comments"
---

### Introduction

In our previous works, we developed a command-line based pipeline in Java to identify various information types from class comments \[1\]. The pipeline preprocesses the comments stored in database, process them, and prepares a machine-learning based classification model.  In another follow-up work \[2\], we developed a JavaScript-based web browser plugin that identifies the comments from a file in a GitHub repository and classify it into various categories or information types.

The aim of this project is to improve the pipeline in classifying the comments and make a working prototype tool to help developers get an overview of what their comments contain.

### Steps

1.  Identify code comments of open-source projects.
2.  Scrape the comments and feed them to supervised machine learning models (already prepared) and deep learning models to classify them.
3.  Compare the performance of supervised machine learning models and deep learning models.
4.  Show the classified comments to developers.
5.  Ask developers to label the comments if the information is identified correctly or not.
6.  Improve the models based on the labeled data (continuous training and feedback).

### Activities

⬤⬤⬤⬤◯ Programming

⬤⬤⬤⬤◯ Experimentation

⬤◯◯◯◯ Literature

### Prerequisites

Java (to understand the existing pipeline)

Abstract Syntax Tree (to extract comments)

HTML/CSS/JavaScript (to develop web extension)

Choice for the technology can be further discussed.

### Contact

[Pooja Rani](https://seg.inf.unibe.ch/people/pooja/), [Joel Niklaus](https://www.digitale-nachhaltigkeit.unibe.ch/about_us/persons/niklaus_joel/index_eng.html)

### References

\[1\] [https://www.sciencedirect.com/science/article/pii/S0164121221001448?via%3Dihub](https://www.sciencedirect.com/science/article/pii/S0164121221001448?via%3Dihub)
\[2\] [http://scg.unibe.ch/wiki/projects/mastersbachelorsprojects/Develope-interface-cli-classify-comments](http://scg.unibe.ch/wiki/projects/mastersbachelorsprojects/Develope-interface-cli-classify-comments)