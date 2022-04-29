---
title: "Explainability Annotations for Legal Judgment Prediction in Switzerland"
---

### Introduction

We recently presented a dataset for Legal Judgment Prediction (you try to predict the outcome of a case based on its facts) including 85K Swiss Federal Supreme Court decisions \[2\]. Although we achieved up to 80% Macro-F1 Score, the models still work as black boxes and are thus not interpretable. In this project, you will work together with a legal student, to annotate some decisions in the dataset for explainability. You will use the annotation tool [Prodigy](https://prodi.gy/) and write annotation guidelines for collecting high-quality annotations.

### Research Questions

So far, to the best of our knowledge, the Explainable AI methods have not been studied in Swiss Legal Judgment Prediction.

RQ1: To what extent do current models predict the judgment outcome based on input deemed important by lawyers?

### Steps

1.  Get familiar with the literature on explainable NLP.
2.  Write the annotation guidelines.
3.  Set up Prodigy for the annotation process.
4.  Work together with the law student to collect the annotations.
5.  Analyze the annotated data and run experiments based on the annotations.
6.  Describe the annotation process and the annotated data in detail.

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
\[2\] Niklaus, J et al. "Swiss-Judgment-Prediction: A Multilingual Legal Judgment Prediction Benchmark" Natural Legal Language Processing Workshop @ Empirical Methods for Natural Language Processing (2021)
\[3\] Malik, V., Sanjay, R., Nigam, S.K., Ghosh, K., Guha, S.K., Bhattacharya, A., & Modi, A. (2021). ILDC for CJPE: Indian Legal Documents Corpus for Court JudgmentPrediction and Explanation. _ACL/IJCNLP_.