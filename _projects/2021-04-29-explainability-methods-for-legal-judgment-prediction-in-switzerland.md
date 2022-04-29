---
title: "Explainability Methods for Legal Judgment Prediction in Switzerland"
dataset: "#"
code: "#"
---

### Introduction

We recently presented a dataset for [Legal Judgment Prediction](https://github.com/joelniklaus/swissjudgementprediction) (you try to predict the outcome of a case based on its facts) including 85K Swiss Federal Supreme Court decisions \[2\]. Although we achieved up to 70% Macro-F1 Score, the models still work as black boxes and are thus not interpretable. In this project, you will venture in the realm of explainable Machine Learning to understand the predictions better the models made on the Legal Judgment Prediction dataset. There are many explainability methods that can be tried and compared such as [SHAP](https://github.com/slundberg/shap), [LIME](https://github.com/marcotcr/lime/issues/356), [Diverse Counterfactual Explanations](https://github.com/interpretml/DiCE), Integrated Gradients, [using Attention](https://medium.com/analytics-vidhya/explainability-of-bert-through-attention-7dbbab8a7062), or using [Probes](https://youtu.be/HJn-OTNLnoE) to predict the legal area, origin cantons or citations.

Other libraries that might come in handy: [Interpret-text](https://github.com/interpretml/interpret-text), [Captum](https://captum.ai/), [transformers-interpret](https://github.com/cdpierse/transformers-interpret)

### Research Questions

So far, to the best of our knowledge, the Explainable AI methods have not been studied in Swiss Legal Judgment Prediction.

RQ1: Can we find the models relying on spurious correlations, rather than on sensible content, to make the decisions?

RQ2: What insight on the prediction of the legal judgment outcome can we draw using the explanations?

### Steps

1.  Get roughly familiar with the literature on explainable NLP.
2.  Get roughly familiar with the existing code for [Swiss Judgment Prediction](https://github.com/joelniklaus/swissjudgementprediction).
3.  Get familiar with the explainability method(s) that you will try on the Swiss Judgment Prediction models.
4.  Write the code to test the chosen explainability method(s) on the models.
5.  Analyze the results qualitatively and quantitatively if possible.

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