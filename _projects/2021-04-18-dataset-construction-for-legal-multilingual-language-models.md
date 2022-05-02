---
title: "Dataset Construction for Legal Multilingual Language Models"
article: "#"
print: "#"
dataset: "#"
code: "#"
models: "#"
---

### Introduction

Since legal text is often rather long, conventional transformer-based models are not optimal in this area. Various _efficient_ transformer variants have been proposed \[2\]. However, none of these models has been pretrained in languages other than English so far. Additionally, models pretrained on legal data are rather rare and do not exist for the Swiss national languages so far. To pretrain an efficient multilingual transformer-based model capable of handling long text input on legal data, many corpora need to be collected.

List of possible data sources:

*   [European Court of Human Rights](#)
*   [Legislation from European Countries](https://e-justice.europa.eu/6/EN/national_legislation)
*   [Case Law from European Countries](https://e-justice.europa.eu/content_ecli_search_engine-430-en.do)
*   others