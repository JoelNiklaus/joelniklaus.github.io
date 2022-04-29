---
title: "Section Splitting for Swiss Court Rulings"
article: "#"
print: "#"
dataset: "#"
code: "#"
models: "#"
---

### Introduction

Section splitting (aka text segmentation or text zoning) is an NLP task that splits a larger text into several coherent subunits. In our case, we want to split Swiss court decisions into the sections _rubrum, facts, considerations,_ and _rulings_. These sections serve different purposes and are required for downstream tasks such as legal judgment prediction or citation prediction.

### Example

From the recent decision of the Swiss Federal Supreme Court [9C\_502/2017](https://tinyurl.com/mjxfjn65):

_Urteil vom 21. September 2017_

_II. sozialrechtliche Abteilung_

_Besetzung_

_Bundesrichterin Pfiffner, Präsidentin,_

_Bundesrichterin Glanzmann, Bundesrichter Parrino,_

_Gerichtsschreiberin Oswald._

_Verfahrensbeteiligte_

 _A.\_\_\_\_\_\_\_\_,_

_vertreten durch Rechtsanwalt Jan Herrmann,_

_Beschwerdeführerin,_

_gegen_

_IV-Stelle Basel-Stadt,_

_Lange Gasse 7, 4052 Basel,_

_Beschwerdegegnerin._

_Gegenstand_

_Invalidenversicherung_

_(vorinstanzliches Verfahren; Prozessvoraussetzung),_

_Beschwerde gegen den Entscheid des Sozialversicherungsgerichts des Kantons Basel-Stadt vom 10. Juni 2017 (IV.2016.186)._

_Nach Einsicht_

_in die Beschwerde vom 18. Juli 2017 (Poststempel) gegen den Entscheid des Sozialversicherungsgerichts des Kantons Basel-Stadt vom 10. Juni 2017, mit welchem auf das Gesuch vom 21. November 2016 um Revision des Entscheids vom 11. Oktober 2016 nicht eingetreten wurde,_

_in Erwägung,_

_dass das kantonale Gericht erkannte, das einschlägige Prozessrecht (§ 18 Abs. 1 lit. a des Gesetzes über das Sozialversicherungsgericht des Kantons Basel-Stadt und über das Schiedsgericht in Sozialversicherungssachen vom 9. Mai 2001 \[Sozialversicherungsgerichtsgesetz, SVGG/BS SGS 154.200\]) sehe die Revision unter anderem bei Entdeckung neuer erheblicher Tatsachen oder Beweismittel vor (Art. 61 lit. i ATSG),_

_dass es erwog, beim Revisionsgesuch handle es sich um ein ausserordentliches Rechtsmittel, das sich gegen einen rechtskräftigen Beschwerdeentscheid richte, ein solcher jedoch vorliegend nicht gegeben sei, da die Gesuchstellerin gegen den Entscheid des Sozialversicherungsgerichts Basel-Stadt vom 11. Oktober 2016 Beschwerde beim Bundesgericht erhoben habe,_

_dass diese Beschwerde vom 21. November 2016 beim Bundesgericht noch hängig ist (9C\_782/2016),_

_dass eine Vorinstanz des Bundesgerichts auf ein Revisionsgesuch nicht einzig mit der Begründung nicht eintreten darf, gegen den zu revidierenden Entscheid sei Beschwerde beim Bundesgericht erhoben worden ([BGE 138 II 386](https://www.bger.ch/ext/eurospider/live/de/php/aza/http/index.php?lang=de&type=highlight_simple_query&page=1&from_date=&to_date=&sort=relevance&insertion_date=&top_subcollection_aza=all&query_words=9C_502%2F2017&rank=0&azaclir=aza&highlight_docid=atf%3A%2F%2F138-II-386%3Ade&number_of_ranks=0#page386) E. 6 S. 389 ff.; Urteil 8C\_921/2014 vom 12. Mai 2015 E. 2.3),_

_dass die Beschwerde damit offensichtlich begründet und deshalb im Verfahren nach Art. 109 Abs. 2 lit. b BGG mit summarischer Begründung (Art. 109 Abs. 3 Satz 1 BGG) gutzuheissen ist,_

_dass umständehalber auf die Erhebung von Gerichtskosten zu verzichten ist (Art. 66 Abs. 1 Satz 2 BGG),_

_Demnach erkennt das Bundesgericht:_

_1.   Die Beschwerde wird gutgeheissen. Der Entscheid des Sozialversicherungsgerichts des Kantons Basel-Stadt vom 10. Juni 2017 wird aufgehoben. Die Sache wird an die Vorinstanz zurückgewiesen, damit sie über die übrigen Eintretensvoraussetzungen bezüglich des Gesuchs vom 21. November 2016 entscheide und dieses gegebenenfalls materiell behandle._

_2.   Es werden keine Gerichtskosten erhoben._

_3.   Die Beschwerdegegnerin hat die Beschwerdeführerin für das bundesgerichtliche Verfahren mit Fr. 2'000.- zu entschädigen._

_4.   Dieses Urteil wird den Parteien, dem Sozialversicherungsgericht des Kantons Basel-Stadt und dem Bundesamt für Sozialversicherungen schriftlich mitgeteilt._

_Luzern, 21. September 2017_

_Im Namen der II. sozialrechtlichen Abteilung_

_des Schweizerischen Bundesgerichts_

_Die Präsidentin: Pfiffner_

_Die Gerichtsschreiberin: Oswald_

You would split the text into the following sections:

rubrum

facts

considerations

judgment

### Research Questions

Apart from the Federal Supreme Court of Switzerland, there does not exist section splitting for Swiss court decisions.

RQ1: To what extent can regular expressions and parsers be used to split Swiss court decisions into sections?

RQ2: What coverage can be achieved? (i.e. for how many decisions could we split sections successfully?)

### Steps

1.  Select large Swiss courts (e.g. Bundesverwaltungsgericht, Zürich Sozialversicherungsgericht)
2.  Analyze the structure of decisions and look for patterns that identify section boundaries
3.  Implement parsers and regular expressions splitting the decisions based on the identified patterns
4.  Calculate the section splitting coverage (e.g. for how many decisions did we identify facts)

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