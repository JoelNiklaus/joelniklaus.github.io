---
title: "Topic Modeling for Swiss Court Rulings"
article: "#"
print: "#"
dataset: "#"
code: "#"
models: "#"
---

### Introduction

Topic Modeling is a text-mining tool used to capture hidden semantics in texts. It clusters documents into topics based on similar words. Eventually, the topics discovered may guide the search for external data required for the re-identification of a given court ruling.

### Research Questions

So far, Swiss court decisions have not been analyzed for their abstract topics.

RQ1: Which topic model provides the most coherent topics on Swiss court rulings?

RQ2: What conclusions can be drawn from the topic model and its visualizations?

### Steps

1.  Preprocess the data (Swiss German Federal Court Rulings)
2.  Build the topic model (e.g. with [BERTopic](https://github.com/MaartenGr/BERTopic/) or [contextualized-topic-models](https://github.com/MilaNLProc/contextualized-topic-models))
3.  Experiment with different topic models (LDA, NMF, BERTopic etc.), different numbers of topics, and other hyperparameters
4.  Visualize the results (e.g. with [lda-vis](https://github.com/bmabey/pyLDAvis))
5.  Evaluate the results

### Activities

⬤⬤⬤⬤◯ Programming

⬤⬤⬤⬤◯ Experimentation

⬤◯◯◯◯ Literature

### Prerequisites

Good programming skills (preferably in Python)

Preferably experience with Machine Learning

### Contact

[Joel Niklaus](https://www.digitale-nachhaltigkeit.unibe.ch/about_us/persons/niklaus_joel/index_eng.html)

### References

\[1\] Vokinger, K.N., Mühlematter, U.J., 2019. Re-Identifikation von Gerichtsurteilen durch «Linkage» von Daten(banken). Jusletter 27.