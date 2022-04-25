---
title: "Re-Identification in Court Decisions with Knowledge Graphs"
---

Re-Identification in Court Decisions with Knowledge Graphs
----------------------------------------------------------

This project is available as a Master's project.

### Introduction

Swiss court decisions are anonymized to protect the privacy of the involved people (parties, victims, etc.). Previous research \[1\] has shown that it is possible to re-identify companies involved in court decisions by linking the rulings with external data in certain cases. Our project tries to further build an automated system for re-identifying involved people from court rulings. This system can then be used as a test for the anonymization practice of Swiss courts. For more information regarding the overarching research project please [go here](https://www.digitale-nachhaltigkeit.unibe.ch/index_eng.html).

We propose to approach the general problem of re-identification (not only for a specific domain) with knowledge graphs (ontologies). In a first step, you will construct knowledge graphs from both external data and court decisions. Then you will perform ontology alignment \[2\] to connect the two knowledge graphs (a big one from external data and a small one from the court decision to be re-identified). An anonymized node from the knowledge graph of the court decision being aligned to a node from the external data knowledge graph is a re-identification. In a last step, you will analyze the success of your system by measuring the recall and precision of the re-identifications.

### Research Questions

So far, to the best of our knowledge, no one has tried re-identifying individuals occurring in court decisions with ontology alignment.

RQ1: How many individuals can be re-identified using ontology alignment (recall)?

RQ2: What percentage of re-identifications are actually correct (precision)?

### Steps

1.  Construct a knowledge graph from external data like newspaper articles (data is already available)
2.  Construct knowledge graphs from court decisions
3.  Perform ontology alignment between the knowledge graph from the court decision and the one from the external data
4.  Detect and verify re-identifications
5.  Analyze the experimental results

### Activities

⬤⬤⬤◯◯ Programming

⬤⬤⬤⬤◯ Experimentation

⬤◯◯◯◯ Literature

### Prerequisites

Good programming skills (preferably in Python)

Preferably experience in deep learning (transformers)

### Contact

[Joel Niklaus](https://www.digitale-nachhaltigkeit.unibe.ch/about_us/persons/niklaus_joel/index_eng.html)

### References

\[1\] Vokinger, K.N., Mühlematter, U.J., 2019. Re-Identifikation von Gerichtsurteilen durch «Linkage» von Daten(banken). Jusletter 27.
\[2\] Iyer, Vivek, Arvind Agarwal and Harshit Kumar. “VeeAlign: a supervised deep learning approach to ontology alignment.” _OM@ISWC_ (2020).