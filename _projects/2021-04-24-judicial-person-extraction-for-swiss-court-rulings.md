---
title: "Judicial Person Extraction for Swiss Court Rulings"
---

### Introduction

We group parties (with their legal counsels), lawyers, clerks, and judges involved in a court decision as _judicial persons_. We define the Judicial Person Extraction task as follows: Extracting judicial persons' names, gender, and occupation from court decisions. The results of this task can be used to study bias in the judicial system (e.g. lawyers of a specific gender are more successful at a specific court, are men more likely to go to prison?) This project will extract judicial persons from the rubrum (header) of Swiss court decisions.

### Example

From the rubrum of the decision of the Zurich Administrative Court [AB.2009.00001](https://entscheidsuche.ch/docs/ZH_Verwaltungsgericht/ZH_VG_001_-AB-2009-00001_13-01-2010.html):

_Beschluss_

_der 4. Kammer_

_vom 13\. Januar 2010_

_Mitwirkend: Abteilungspräsident Jso Schumacher (Vorsitz), Verwaltungsrichter Lukas Widmer, Verwaltungsrichterin Maja Schüpbach Schmid, Gerichtssekretär Philip Conradin._

_In Sachen_

_A,
vertreten durch Rechtsanwalt B,_

_Beschwerdeführerin,_

_gegen_

_Staat Zürich,
vertreten durch die Volkswirtschaftsdirektion des Kantons Zürich,_

_Beschwerdegegner,_

_betreffend Aufsichtsbeschwerde / Kostenauflage,_

You would extract the following JSON:

{

"president": {"firstname": "Jso", "lastname": "Schumacher", "gender": "male"},

"judges": \[{"firstname": "Lukas", "lastname": "Widmer", "gender": "male"}, {"firstname": "Maja", "lastname": "Schüpbach Schmid", "gender": "female"}\],

"clerks": \[{"firstname": "Philip", "lastname": "Conradin", "gender": "male"}\],

"complainant": \[{"name": "A", "legal counsel": "B"}\],

"respondent": \[{"name": Volkswirtschaftsdirektion des Kantons Zürich"}\]

}

### Research Questions

Apart from the Federal Supreme Court of Switzerland, extracted judicial persons do not exist for Swiss court decisions.

RQ1: To what extent can regular expressions and parsers be used to extract judicial persons from Swiss court decisions?

RQ2: What coverage can be achieved? (i.e. how many judicial persons can be extracted with their attributes?)

### Steps

1.  Select large Swiss courts (e.g. Bundesverwaltungsgericht, Zürich Sozialversicherungsgericht)
2.  Analyze the structure of the rubrum and look for patterns that identify the different judicial persons
3.  Implement parsers and regular expressions extracting the judicial persons based on the identified patterns
4.  Calculate the judicial person extraction coverage (e.g. for how many decisions did we find at least one judicial person or how many percent of judicial persons can be extracted based on a few manually annotated samples)

### Activities

⬤⬤⬤⬤◯ Programming

⬤⬤⬤◯◯ Experimentation

⬤◯◯◯◯ Literature

### Prerequisites

Good programming skills (preferably in Python)

Preferably experience with regular expressions

### Contact

[Joel Niklaus](https://www.digitale-nachhaltigkeit.unibe.ch/about_us/persons/niklaus_joel/index_eng.html)

### References

\[1\] Vokinger, K.N., Mühlematter, U.J., 2019. Re-Identifikation von Gerichtsurteilen durch «Linkage» von Daten(banken). Jusletter 27.