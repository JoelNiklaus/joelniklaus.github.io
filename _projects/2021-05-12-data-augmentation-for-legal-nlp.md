---
title: "Data Augmentation for Legal NLP"
dataset: "#"
code: "#"
---

### Introduction

Legal Judgment Prediction is an NLP task that automatically predicts the judgment outcome based on the facts of a case. In our dataset, we only have around 4K Italian decisions but more than 31K French decisions and almost 50K German decisions. As can be expected, the performance on the Italian dataset is much worse compared to the French and German dataset. In this project, you will experiment with data augmentation techniques \[2\] such as back-translation or machine-translating decisions from high-resource (many data points) languages (German and French in our case) to low-resource (few data points) languages (Italian in our case).

### Research Questions

The literature on data augmentation in NLP is thin and almost non-existent in legal NLP.

RQ1: What data augmentation techniques are most promising to improve the performance in legal judgment prediction?

RQ2: To what extent does it help more in the low-resource setting compared to the high-resource setting?

### Steps

1.  Identify the most promising data augmentation techniques in imbalanced text classification.
2.  Introduce the selected data augmentation techniques into the legal judgment prediction training pipeline (maybe using [nlpaug](https://github.com/makcedward/nlpaug)).
3.  Run experiments to test the benefit of using the selected techniques.
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
\[2\] Feng, Steven et al. “A Survey of Data Augmentation Approaches for NLP.” Findings of the Association for Computational Linguistics: ACL-IJCNLP 2021 (2021): n. pag. Crossref. Web.