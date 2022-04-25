---
title: "Zero-Shot and Few-Shot Natural Language Inference Models for Judgment Prediction"
---

Zero-Shot and Few-Shot Natural Language Inference Models for Judgment Prediction
--------------------------------------------------------------------------------

This project is available as a Seminar project. This project is also available as a group project.

### Introduction

Swiss court decisions are anonymized to protect the privacy of the involved people (parties, victims, etc.). Previous research \[1\] has shown that it is possible to re-identify companies involved in court decisions by linking the rulings with external data in certain cases. Our project tries to further build an automated system for re-identifying involved people from court rulings. This system can then be used as a test for the anonymization practice of Swiss courts. For more information regarding the overarching research project please [go here](https://www.digitale-nachhaltigkeit.unibe.ch/index_eng.html).

Formulating text classification as a Natural Language Inference (NLI) task \[2\] enables strong Zero-Shot and Few-Shot performance in text classification tasks. The aim of this project is to apply this method to the multilingual Swiss Judgment Prediction benchmark \[3\].

### Research Questions

So far, to the best of our knowledge, the Zero-Shot and Few-Shot classification using Natural Language Inference Models has not been studied on the legal judgment prediction task.

RQ1: What Macro-F1 Score (a way to measure the performance of a model) can be achieved using Natural Language Inference Models in the Zero-Shot and Few-Shot setting on the Swiss Judgment Prediction benchmark?

RQ2: What biases does the model exhibit concerning different cantons, legal areas, or publication years? (So, e.g. is it better in certain cantons than in others?)

### Steps

1.  Get into the topic (further resources: [https://nlp.town/blog/zero-shot-classification/](https://nlp.town/blog/zero-shot-classification/), [https://joeddav.github.io/blog/2020/05/29/ZSL.html](https://joeddav.github.io/blog/2020/05/29/ZSL.html), [https://aclanthology.org/2021.acl-short.99.pdf](https://aclanthology.org/2021.acl-short.99.pdf))
2.  Set up the experiment pipeline for the Swiss Legal Judgment Prediction task
3.  Experiment with different models: [https://huggingface.co/joeddav/xlm-roberta-large-xnli](https://huggingface.co/joeddav/xlm-roberta-large-xnli), [https://huggingface.co/MoritzLaurer/mDeBERTa-v3-base-mnli-xnli](https://huggingface.co/MoritzLaurer/mDeBERTa-v3-base-mnli-xnli), [https://huggingface.co/facebook/bart-large-mnli](https://huggingface.co/facebook/bart-large-mnli)
4.  Consider comparing it with other methods for Zero-Shot and Few-Shot classification
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
\[2\] Yin, W., Hay, J., & Roth, D. (2019). Benchmarking Zero-shot Text Classification: Datasets, Evaluation and Entailment Approach. _ArXiv, abs/1909.00161_.
\[3\] Joel Niklaus, Ilias Chalkidis, and Matthias Stürmer. 2021. [Swiss-Judgment-Prediction: A Multilingual Legal Judgment Prediction Benchmark](https://aclanthology.org/2021.nllp-1.3). In _Proceedings of the Natural Legal Language Processing Workshop 2021_, pages 19–35, Punta Cana, Dominican Republic. Association for Computational Linguistics.