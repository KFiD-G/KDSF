[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

[![KDSF-Logo](https://kerndatensatz-forschung.de/img/logo_kdsf.png)](https://kerndatensatz-forschung.de/)
# KDSF – Standard für Forschungsinformationen in Deutschland
In diesem Repositorium befinden sich ein exemplarisches Austauschformat und ein exemplarisches Datenmodell für den [KDSF](https://kerndatensatz-forschung.de/) Version 1.3. Der KDSF ist ein Standard für Forschungsinformationen für das deutsche Wissenschaftssystem. Er stellt ein freiwilliges Regelwerk zur Harmonisierung und Standardisierung der Forschungsberichterstattung an Forschungseinrichtungen dar. 

Häufig gestellte Fragen zum KDSF-Standard im Allgemeinen sowie zum Einführungsprozess des KDSF werden in den [FAQs](https://kerndatensatz-forschung.de/index.php?id=hd_faq) beantwortet.
### Bitte beachten Sie:
Das exemplarische Austauschformat und das exemplarische Datenmodell in diesem Repositorium entsprechen **nicht** dem [KDSF](https://kerndatensatz-forschung.de/)-Datenmodell Version 2.0. Stand Januar 2025 steht noch nicht fest, ob und welcher Weise eine Aktualisierung des Austauschformats erfolgen wird. Eine formale Modellierung des KDSF Version 2.0 wird angestrebt.

## Austauschformat (XML-Schema)
Das XML-Schema definiert ein Datenaustauschformat für den KDSF Version 1.3, das zum Austausch von Forschungsinformationen zwischen einer Forschungseinrichtung und einer datenabfragenden Stelle genutzt werden kann. Das Schema basiert auf dem [CERIF-Standard](https://www.eurocris.org/services/main-features-cerif).
Das Schema besteht aus zwei Teilen:
* [kdsf-basis.xsd](https://github.com/KFiD-G/KDSF/blob/main/kdsf-basis.xsd) (XML-Schema für die Basisdaten)
* [kdsf.xsd](https://github.com/KFiD-G/KDSF/blob/main/kdsf.xsd) (XML-Schema für die Aggregatdaten)
Darüber hinaus gibt es einige [Klassifikationsschemata](https://github.com/KFiD-G/KDSF/blob/main/kdsf-cerif-classes.xml), die gemäß dem CERIF-Standard definiert wurden. Die Klassifikationsschemata enthalten die für das deutsche Forschungssystem typischen Objekte (z.B. Personalkategorien, Mittelgeber). Ein XML-Dokument im Format des KDSF sollte diese Klassifikationsschemata benutzen. Die Klassifikationsschemata sind in [kdsf-cerif-classes.xml](https://github.com/KFiD-G/KDSF/blob/main/kdsf-cerif-classes.xml) definiert.
### Bitte beachten Sie:
Das exemplarisches Austauschformat ist möglicherweise unvollständig. Das XML-Schema für die Basisdaten ist keine vollständige Modellierung der Basisdaten, die für die Bildung der Aggregate des KDSF Version 1.3 notwendig sind.
## Formales Datenmodell (OWL)
Die OWL-Dateien repräsentieren exemplarisch ein Datenmodell für den KDSF Version 1.3. Die Modellierung besteht aus drei Teilen:
*	[kdsf.owl](https://github.com/KFiD-G/KDSF/blob/main/kdsf.owl) (Basismodell mit den grundlegenden Konzepten für Forschungsinformationen)
*	[kdsf-aggr.owl](https://github.com/KFiD-G/KDSF/blob/main/kdsf-aggr.owl) (Model der Aggregatdaten mit Objekten, die Werte aus dem Basismodell aggregieren)
*	[kdsf-meta.owl](https://github.com/KFiD-G/KDSF/blob/main/kdsf-meta.owl) (Metamodell mit der Definition zweier Meta-Konstrukte, die in den Modellen genutzt werden)
### Bitte beachten Sie:
Die Modellierung des KDSF in Gestalt der OWL-Dateien ist unvollständig und die IRIs lassen sich nicht derefenzieren. Eine formale Modellierung des KDSF Version 2.0 wird angestrebt. Maßgeblich für den KDSF ist das Datenmodell der Version 2.0.
## Kontakt und Anfragendokumentation
Die Geschäftsstelle der Kommission für Forschungsinformationen in Deutschland (KFiD) nimmt gern Ihre [Anfragen](https://kerndatensatz-forschung.de/hd_benutzer/index.php) zum KDSF-Standard und seinen Definitionen entgegen und dokumentiert ausgewählte Fragen und Antworten in einer öffentlich einsehbaren [Anfragendokumentation](https://kerndatensatz-forschung.de/index.php?id=anfragedoku).
Für Rückmeldungen und Fragen, die unmittelbar die Dateien in diesem Repositorium betreffen, erstellen Sie bitte ein neues [Issue](https://github.com/KFiD-G/KDSF/issues). 
