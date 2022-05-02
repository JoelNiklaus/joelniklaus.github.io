---
title: "Explainability Methods for Legal Judgment Prediction in Switzerland"
article: "#"
print: "#"
dataset: "#"
code: "#"
models: "#"
---

### Introduction

We recently presented a dataset for [Legal Judgment Prediction](https://github.com/joelniklaus/swissjudgementprediction) (you try to predict the outcome of a case based on its facts) including 85K Swiss Federal Supreme Court decisions \[2\]. Although we achieved up to 70% Macro-F1 Score, the models still work as black boxes and are thus not interpretable. In this project, you will venture in the realm of explainable Machine Learning to understand the predictions better the models made on the Legal Judgment Prediction dataset. There are many explainability methods that can be tried and compared such as [SHAP](https://github.com/slundberg/shap), [LIME](https://github.com/marcotcr/lime/issues/356), [Diverse Counterfactual Explanations](https://github.com/interpretml/DiCE), Integrated Gradients, [using Attention](https://medium.com/analytics-vidhya/explainability-of-bert-through-attention-7dbbab8a7062), or using [Probes](https://youtu.be/HJn-OTNLnoE) to predict the legal area, origin cantons or citations.

Other libraries that might come in handy: [Interpret-text](https://github.com/interpretml/interpret-text), [Captum](https://captum.ai/), [transformers-interpret](https://github.com/cdpierse/transformers-interpret)