---
title: "Re-Identification with Data from the Swiss Transportation Safety Investigation Board"
---

### Introduction

Legal Judgment Prediction is an NLP task that automatically predicts the judgment outcome based on the facts of a case. In this project, you will extract the judgment outcomes from the rulings of Swiss court decisions. This forms the basis for the judgment prediction task.

### Example

From the judgment of the recent decision of the Swiss Federal Administrative Court [A-1004/2020, A-1022/2020](https://entscheidsuche.ch/docs/CH_BVGer/CH_BVGE_001_A-1004-2020_2021-07-07.pdf):

_Demnach erkennt das Bundesverwaltungsgericht:_

_1\. Auf die Beschwerden wird nicht eingetreten._

_2\. Ein Verfahrenskostenanteil von Fr. 1'500.-- wird der Beschwerdeführerin 1 auferlegt. Dieser Betrag wird dem von der Beschwerdeführerin 1 geleisteten Kostenvorschuss entnommen._

_3\. Die Beschwerdeführerin 1 wird verpflichtet, dem Beschwerdegegner eine Parteientschädigung in der Höhe von Fr. 4'000.-- zu bezahlen._

_4\. Die Beschwerdeführerin 2 wird verpflichtet, dem Beschwerdegegner eine Parteientschädigung in der Höhe von Fr. 4'000.-- zu bezahlen._

_5\. Dieses Urteil geht an:_

_– die Beschwerdeführerin 1 (Gerichtsurkunde)_

_– die Beschwerdeführerin 2 (Gerichtsurkunde)_

_– den Beschwerdegegner (Gerichtsurkunde)_

_– die Vorinstanz (Ref-Nr. \[…\]; Einschreiben)_

_– das UVEK (Gerichtsurkunde)_

_Für die Rechtsmittelbelehrung wird auf die nächste Seite verwiesen._

You would recognize the underlined part and conclude that the judgment outcome is: inadmissible (Nichteintreten)

### Research Questions

Apart from the Federal Supreme Court of Switzerland, there do not exist extracted judgment outcomes for Swiss court decisions.

RQ1: To what extent can regular expressions and parsers be used to extract judgments from Swiss court decisions?

RQ2: What coverage can be achieved? (i.e. how many judgment outcomes can be extracted?)

### Steps

1.  Select large Swiss courts (e.g. Bundesverwaltungsgericht, Zürich Sozialversicherungsgericht)
2.  Analyze the structure of the rulings and look for patterns that identify the different judgment outcomes
3.  Implement parsers and regular expressions extracting the judgment outcomes based on the identified patterns
4.  Calculate the judgment extraction coverage (e.g. for how many decisions did we find at least one judgment outcome)

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