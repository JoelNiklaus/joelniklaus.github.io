---
title: "Re-Identification with Data from the Swiss Transportation Safety Investigation Board"
---

Re-Identification with Data from the Swiss Transportation Safety Investigation Board
------------------------------------------------------------------------------------

This project is available as a Seminar project.

### Introduction

Swiss court decisions are anonymized to protect the privacy of the involved people (parties, victims, etc.). Previous research \[1\] has shown that in certain cases, it is possible to re-identify companies involved in court decisions by linking the rulings with external data. Our project tries to go a step further by building an automated system for re-identifying involved people from court rulings. This system can then be used as a test for the anonymization practice of Swiss courts. For more information regarding the overarching research project, please [go here](./../../../../index_eng.html).

There are court decisions tackling all kinds of accidents, such as accidents involving trains, cars, and airplanes. Such accidents are also described on the website of Swiss Transportation Safety Investigation Board (STSB). The aim of this project is to find out, to what extent this information can be used to re-identify entities occurring in court decisions.

### Research Questions

So far, to the best of our knowledge, no one tried to re-identify entities in court decision using data from the Swiss Transportation Safety Investigation Board.

RQ1: Is it possible to re-identify entities in court decision using data from the Swiss Transportation Safety Investigation Board?

RQ2: How many entities can be re-identified?

### Steps

1.  Explore the STSB data and maybe extract relevant information (maybe using models for tasks such as Named Entity Recognition)
2.  Select promising Swiss court decisions (ones that are related to accidents reported to the STSB)
3.  Make connections between specific accidents reported to the STSB and specific court decisions
4.  Extend these connections to specific entities in the court decisions
5.  Evaluate the results (e.g. how many entities could be re-identified?, how confident can we be about the re-identifications?, what ratio of court decisions are vulnerable?)

### Activities

⬤⬤⬤⬤◯ Programming

⬤⬤◯◯◯ Experimentation

⬤◯◯◯◯ Literature

### Prerequisites

Good programming skills (preferably in Python)

Some experience in deep learning is helpful

### Contact

[Joel Niklaus](https://www.digitale-nachhaltigkeit.unibe.ch/about_us/persons/niklaus_joel/index_eng.html)

### References

\[1\] Vokinger, K.N., Mühlematter, U.J., 2019. Re-Identifikation von Gerichtsurteilen durch «Linkage» von Daten(banken). Jusletter 27.