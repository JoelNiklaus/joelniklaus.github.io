---
title: "Negation Scope Resolution for the Multilingual Legal Domain"
article: "#"
print: "#"
dataset: "#"
code: "#"
models: "#"
---

### Introduction

Negation Scope Resolution describes the task of finding the scope of a negation cue (e.g. "not") in a sentence (see example below). Recent transfer learning techniques such as BERT have been successfully applied on the Negation Scope Resolution task \[2\]. Negation Scope Resolution has been investigated on multilingual data \[3\], but, to the best of our knowledge, not yet in the legal domain.

Decision [8C\_873/2015 {T 0/2}](https://www.bger.ch/ext/eurospider/live/de/php/aza/http/index.php?lang=de&type=highlight_simple_query&page=18&from_date=09.12.2015&to_date=28.12.2015&sort=relevance&insertion_date=&top_subcollection_aza=all&query_words=&rank=179&azaclir=aza&highlight_docid=aza%3A%2F%2F17-12-2015-8C_873-2015&number_of_ranks=418):

dass der vorliegende Begründungsmangel offensichtlich ist, weshalb auf die Beschwerde in Anwendung von Art. 108 Abs. 1 lit. b BGG nicht _einzutreten ist_,
dass von der Erhebung von Gerichtskosten für das bundesgerichtliche Verfahren umständehalber abzusehen ist (Art. 66 Abs. 1 Satz 2 BGG),
dass in den Fällen des Art. 108 Abs. 1 BGG das vereinfachte Verfahren zum Zuge kommt und die Abteilungspräsidentin zuständig ist,

Negation Cue underlined, _Negation Scope_ in italics

### Research Questions

So far, to the best of our knowledge, the performance of Negation Scope Resolution is still subpar in multilingual legal documents

RQ1: What is the performance of current negation scope resolution systems on multilingual legal data

RQ2: To what extent can we improve upon this performance?

### Steps

1.  Get roughly familiar with the literature on Negation Scope Resolution
2.  Select suitable data (diverse legal data (contracts, court decisions, legislation, commentaries, etc.) in multiple languages)
3.  Setup [prodigy](https://prodi.gy/) for negation scope resolution annotations and write annotation guidelines
4.  Annotate and/or supervise the annotation process
5.  Evaluate the performance (probably token-level F1) of existing systems on the newly annotated dataset
6.  Train a new system (probably based on [transformers](https://huggingface.co/docs/transformers/index)) and evaluate it
7.  Analyze the results

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
\[2\] Aditya Khandelwal and Suraj Sawant. 2020. [NegBERT: A Transfer Learning Approach for Negation Detection and Scope Resolution](https://aclanthology.org/2020.lrec-1.704). In _Proceedings of the 12th Language Resources and Evaluation Conference_, pages 5739–5748, Marseille, France. European Language Resources Association.
\[3\] Anastassia Shaitarova and Fabio Rinaldi. 2021. [Negation typology and general representation models for cross-lingual zero-shot negation scope resolution in Russian, French, and Spanish.](https://aclanthology.org/2021.naacl-srw.3). In _Proceedings of the 2021 Conference of the North American Chapter of the Association for Computational Linguistics: Student Research Workshop_, pages 15–23, Online. Association for Computational Linguistics.