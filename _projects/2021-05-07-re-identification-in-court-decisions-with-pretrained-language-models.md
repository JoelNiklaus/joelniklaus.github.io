---
title: "Re-Identification in Court Decisions with Pretrained Language Models"
article: "#"
print: "#"
dataset: "#"
code: "#"
models: "#"
---

### Introduction

We propose to approach the general problem of re-identification (not only for a specific domain) with pretrained language models such as BERT or T5. Roberts et al. \[2\] have shown that T5 can be used to answer questions in a closed book way (without context, solely drawing from the parameters!). We plan to pretrain a large language model on a corpus of documents related to Swiss court decisions (e.g. newspapers) and then fine-tune it on a small dataset of re-identified court decisions. Then we will run it on not re-identified court decisions and analyze the results.

### Research Questions

So far, to the best of our knowledge, no one has tried re-identifying individuals occurring in court decisions with pretrained language models.

RQ1: How many individuals can be re-identified using pretrained language models (recall)?

RQ2: What percentage of re-identifications are actually correct (precision)?

### Steps

1.  Further pretrain a large language model on external data like newspaper articles (data is already available)
2.  Create a small dataset of re-identified court decisions (data is already available).
3.  Finetune the large language model on this dataset. There are different possibilities of framing the task:
    1.  Feed the anonymized court decision to the language model and let it predict the anonymized entity via masked language modeling (like gap filling from primary school) \[3\]
    2.  Rephrase the sentence with the anonymization to a question and feed the question to the language model.
    3.  If necessary, try other approaches of using the language model for re-identification
4.  Detect and verify the re-identifications
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
\[2\] Roberts, A., Raffel, C., & Shazeer, N.M. (2020). How Much Knowledge Can You Pack into the Parameters of a Language Model? _ArXiv, abs/2002.08910_.
\[3\] Kassner, N., Dufter, P., & Schütze, H. (2021). Multilingual LAMA: Investigating Knowledge in Multilingual Pretrained Language Models. _ArXiv, abs/2102.00894_.