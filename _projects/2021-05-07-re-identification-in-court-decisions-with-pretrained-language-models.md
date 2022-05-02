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

