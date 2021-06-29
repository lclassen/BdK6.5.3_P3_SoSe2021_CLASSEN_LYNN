# Aufgabe 1 in BDK6.5.3 (wB/öB) P3 Data Librarianship und Programmierung

## 1. Text-Editor der Wahl
Brackets

Dieser Texteditor wurde bereits für eine andere Lehrveranstaltung installiert und zur Programmierung genutzt. Da sowohl das Programm an sich als auch einige Vorkenntnisse dazu vorhanden waren, wurde sich für Brackets als Editor entschieden.

## 2. Eine Python-Bibliothek
inflecteur 0.1.2

Mit dieser Bibliothek können französische Sätze in andere Zeitformen, Geschlechter oder Zählungen gesetzt werden.
Die Bibliothek könnte demnach genutzt werden, um einzelne Sätze, kürzere Abschnitte oder Verbtabellen vom Präsens ins Futur, vom Singular ins Plural oder von der männlichen in die weiblichen Form zu überführen. Die Nutzung dieser Bibliothek bietet sich an, wenn eine oder mehrere dieser Veränderungen auf Text angewendet werden sollen, die sowohl grammatikalisch korrekt als auch möglichst effizient durchgeführt werden sollen.  

## 3. Eine Fehlermeldung und Ihre Lösung
pmid_data["result"]["title"]

---------------------------------------------------------------------------
KeyError                                  Traceback (most recent call last)
<ipython-input-16-c4d5bcbc477b> in <module>
----> 1 pmid_data["result"]["title"]

KeyError: 'title'

Die Fehlermeldung war darauf zurückzuführen, dass es den Key "title" nicht im Key "result" gab. Bei genauerer Betrachtung der Datenstruktur in "result" konnte festgestellt werden, dass sich noch ein weiterer Key dazwischen befand, der der PMID entpricht. Die korrekte Abfrage lautet demnach:
pmid_data["result"]["31452104"]["title"]

## 4. Was ist JupyterLab?
Bei JuypterLab läuft alles über eine Ansichtsseite, während bei JupyterNotebook ein neuer Tab geöffnet wird, wenn auf ein Notebook zugegriffen wird. 
Die Ansicht von JuypterLab wirkt insgesamt komplexer und "professioneller", wobei auf den ersten Blick die gleichen Funktionen zur Verfügung stehen.
JupyterLab ist die nächste Generation von JupyterNotebook, die eine gleichzeitige Nutzung von Texteditoren, Terminals und Dateimanager in einer gemeinsamen Oberfläche ermöglicht, was JupyterNotebook nicht kann.

## 5. Was ist der große Unterschied zwischen den Webframeworks flask und Django
flask legt den Fokus auf kleine Applikation mit niedrigen Anforderungen, während Django eher für große Projekte geeignet ist. Bei flask kann der Entwickler seine Tools und Komponenten selbst auswählen, bei Django ist dies nicht der Fall, der Entwickler bekommt Tools und Komponenten "vorgesetzt".