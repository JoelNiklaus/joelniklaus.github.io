---
title: "Sentence Boundary Detection for Multilingual Legal Text"
---

### Introduction

Research has shown \[2\], that Sentence Boundary Detection (SBD) is not “solved” yet, especially in informal language and in special domains. Especially in the legal domain, conventional sentence splitting methods are still subpar. Although in German \[3\] recent research worked on mitigating this issue, in many other languages such as French, Italian, Spanish, or Portuguese, SBD is not sufficiently researched, to the best of our knowledge. With this project, we plan to close this gap by creating a dataset for multilingual legal SBD, evaluating the performance of current methods on it, and training a superior model.

### Research Questions

So far, to the best of our knowledge, the performance of Sentence Boundary Detection is still subpar in multilingual legal documents

RQ1: What is the performance of current sentence boundary detection systems on multilingual legal data

RQ2: To what extent can we improve upon this performance?

### Steps

1.  Get roughly familiar with the literature on Sentence Boundary Detection
2.  Select suitable data (diverse legal data (contracts, court decisions, legislation, commentaries, etc.) in multiple languages)
3.  Setup [prodigy](https://prodi.gy/) for legal sentence boundary annotations and write annotation guidelines
4.  Supervise the annotation process
5.  Evaluate the performance (F1 over boundary points) of existing systems on the newly annotated dataset
6.  Train a new system (probably based on [transformers](https://huggingface.co/docs/transformers/index)) and evaluate it
7.  Analyze the results

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
\[2\] Jonathon Read, Rebecca Dridan, Stephan Oepen, and Lars Jørgen Solberg. 2012. [Sentence Boundary Detection: A Long Solved Problem?](https://aclanthology.org/C12-2096). In _Proceedings of COLING 2012: Posters_, pages 985–994, Mumbai, India. The COLING 2012 Organizing Committee.
\[3\] Glaser, I., Moser, S., & Matthes, F. (2021). Sentence Boundary Detection in German Legal Documents. _ICAART_.