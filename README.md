Vorlage für Seminar-Ausarbeitungen
==================================

Bei der Verwendung für Seminare sollten keine Befehle verwendet werden, die das Layout verändern.
Insbesondere sollte die Zeile `\documentclass[10pt,a4paper,sigconf,language=XXX]{acmart}` intakt bleiben.

Folgende Befehle **sollen** angepasst werden:

* `\title{Titel}` -- Titel der Ausarbeitung.
* `\author{...}` -- Name der Autorin/des Autors.
* `\email{...}` -- E-Mail-Adresse der Autorin/des Autors.
* `\acmConference[Seminar Acr.]{Seminar Type Long}{WS/SS XXXX}{Institute of Distributed Systems, Ulm University}` 
- Seminar Acr. = KTT, PRIV, PASF, ATVS oder RTDS
- Seminar Type Long (z.B. *Ausgewählte Themen in Verteilten Systemen*) 
- Semester (z.B. *WS 2021/22*).

Die Vorlage kann wie folgt kompiliert werden:  
`pdflatex ausarbeitung.tex`  
`bibtex ausarbeitung.aux`  
`pdflatex ausarbeitung.tex`  
`pdflatex ausarbeitung.tex`  


Beim Importieren des Projektes in Overleaf, sollte vorher die Datei `.latexmkrc` gelöscht werden. Es dürfen also nur folgende Dateien importiert werden: `ACM-Reference-Format.bst`, `acmart.cls`, `ausarbeitung.tex`, `references.bib`, sowie bei Bedarf die zwei `.tex` Dateien in `sections`.
