---
title: "Dataset Construction for Legal Multilingual Language Models"
---

Dataset Construction for Legal Multilingual Language Models
------------------------------------------------------------

This project is available as a Seminar or Bachelor's project. This project is also available as a group project.

### Introduction

Swiss court decisions are anonymized to protect the privacy of the involved people (parties, victims, etc.). Previous research has shown that in certain cases, it is possible to re-identify companies involved in court decisions by linking the rulings with external data. Our project tries to go a step further by building an automated system for re-identifying involved people from court rulings. This system can then be used as a test for the anonymization practice of Swiss courts. For more information regarding the overarching research project, please [go here](https://www.digitale-nachhaltigkeit.unibe.ch/index_eng.html).

Since legal text is often rather long, conventional transformer-based models are not optimal in this area. Various _efficient_ transformer variants have been proposed. However, none of these models has been pretrained in languages other than English so far. Additionally, models pretrained on legal data are rather rare and do not exist for the Swiss national languages so far. To pretrain an efficient multilingual transformer-based model capable of handling long text input on legal data, many corpora need to be collected.

List of possible data sources:

*   [European Court of Human Rights](https://hudoc.echr.coe.int/fre#{%22tabview%22:[%22document%22)
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