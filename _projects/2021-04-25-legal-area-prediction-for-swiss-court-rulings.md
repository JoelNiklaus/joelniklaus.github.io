---
title: "Legal Area Prediction for Swiss Court Rulings"
article: "#"
print: "#"
dataset: "#"
code: "#"
models: "#"
---

### Introduction

Big Courts like the Swiss Federal Supreme Court have many different departments and chambers each responsible for different legal areas. Therefore, an automatic system, which can route a new complaint directly to the responsible department would be very handy for these courts and free up secretaries' time for more important work. Since we do not have access to the complaints we take the facts of a case as a proxy and coin the task Legal Area Prediction, which predicts the legal area from the facts of a case.

### Research Questions

So far, to the best of our knowledge, the Legal Area Prediction task has not been studied in the literature apart from once on the French Supreme Court \[3\].

RQ1: What Macro-F1 Score (a way to measure the performance of a model) can be achieved using state-of-the-art methods in the new Legal Area Prediction task?

RQ2: What biases does the model exhibit concerning different cantons, legal areas, or publication years? (So, e.g. is it better in certain cantons than in others?)

### Steps

1.  Improve and polish the existing legal prediction dataset
2.  Make a script that is given to you ready to run experiments.
3.  Run experiments and improve the Macro-F1 Score of the model by investigating avenues like the following:
    1.  Combatting class imbalance
    2.  Using data augmentation \[2\]
    3.  Handling long textual input better
    4.  Your own ideas
4.  Analyze the experimental results.

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
\[2\] Feng, Steven et al. “A Survey of Data Augmentation Approaches for NLP.” Findings of the Association for Computational Linguistics: ACL-IJCNLP 2021 (2021): n. pag. Crossref. Web.
\[3\] Şulea, Octavia-Maria et al. “Predicting the Law Area and Decisions of French Supreme Court Cases.” RANLP 2017 - Recent Advances in Natural Language Processing Meet Deep Learning (2017): n. pag. Crossref. Web.