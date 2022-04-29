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

### Research Questions

So far, there does not exist a readily available collection of legal datasets usable for pretraining large language models.

RQ1: Is it possible to compile a readily available collection of legal datasets usable for pretraining large language models?

### Steps

1.  Identify promising data sources
2.  Analyze the HTML and scrape the documents from the websites (using libraries such as [Scrapy](https://scrapy.org/) or [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/))
3.  Extract the text from the documents
4.  Evaluate the results (in the sense of a small descriptive analysis of the content)

### Activities

⬤⬤⬤⬤◯ Programming

⬤⬤◯◯◯ Experimentation

⬤◯◯◯◯ Literature

### Prerequisites

Good programming skills (preferably in Python)

### Contact

[Joel Niklaus](https://www.digitale-nachhaltigkeit.unibe.ch/about_us/persons/niklaus_joel/index_eng.html)

### References

\[1\] Vokinger, K.N., Mühlematter, U.J., 2019. Re-Identifikation von Gerichtsurteilen durch «Linkage» von Daten(banken). Jusletter 27.
\[2\] Yi Tay, Mostafa Dehghani, Dara Bahri, Donald Metzler. Efficient Transformers: A Survey