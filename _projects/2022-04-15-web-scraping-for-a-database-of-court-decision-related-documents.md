---
title: "Web Scraping for a Database of Court Decision Related Documents"
---

Web Scraping for a Database of Court Decision Related Documents
---------------------------------------------------------------

This project is available as a Seminar or Bachelor's project. This project is also available as a group project.

### Introduction

Swiss court decisions are anonymized to protect the privacy of the involved people (parties, victims, etc.). Previous research \[1\] has shown that in certain cases it is possible to re-identify companies involved in court decisions by linking the rulings with external data. Our project tries to go a step further by building an automated system for re-identifying involved people from court rulings. This system can then be used as a test for the anonymization practice of Swiss courts. For more information regarding the overarching research project please [go here](https://www.digitale-nachhaltigkeit.unibe.ch/index_eng.html).

For a successful re-identification of involved people in a court decision, we need external data. This project has the goal of building a well-structured database of external data connected to Swiss federal court rulings.

List of possible data sources:

*   Media messages of the courts (e.g. the [federal court](https://www.bger.ch/index/press/press-inherit-template/press-mitteilungen.htm?histo=true))
*   [BAG Bulletin](ttps://www.bag.admin.ch/bag/de/home/das-bag/publikationen/periodika/bag-bulletin.html)
*   [Swiss Transporation Safety Investigation Board](https://www.sust.admin.ch/en/stsb-homepage/)
*   Newspapers (SRF, swissdox, etc.)
*   Online phone books (e.g. local.ch)
*   Social Media (e.g. Twitter, Facebook)
*   Government documents
*   Trade registers/Business register (e.g. Moneyhouse)
*   Map Information systems/Land register

### Research Questions

So far, there has not been collected a dataset of external documents related to Swiss federal court rulings.

RQ1: Which data sources are most likely to contain information also occurring in Swiss federal court rulings?

### Steps

1.  Identify promising data sources
2.  Analyze the HTML and scrape the documents from the websites (using libraries such as [Scrapy](https://scrapy.org/) or [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/))
3.  Extract the text from the documents
4.  Structure the documents in a database
5.  Evaluate the results

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