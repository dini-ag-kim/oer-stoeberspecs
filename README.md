# OER-StöberSpecs

## Werkzeuge und Verfahren zur Standardisierung von OER-Metadaten

Ausgestattet mit Fördermitteln von Bund und Ländern beschäftigen sich immer mehr Akteure und Projekte mit dem Aufbau von Infrastrukturen zur Erstellung, Publikation und zum Teilen von [Open Educational Resources (OER)](https://de.wikipedia.org/wiki/Open_Educational_Resources). Innerhalb einer solchen Infrastruktur spielen Metadaten – strukturierte Beschreibungen, die Informationen über bestimmte Merkmale der beschriebenen Dinge erfassen – eine zentrale Rolle.

Dementsprechend stellt sich derzeit in verschiedenen Kontexten die Frage, wie OER mit Metadaten versehen werden sollten, seit neuestem auch in der im Aufbau befindlichen KMK-Arbeitsgruppe *OER-Repositorien*. Damit keine Parallelarbeiten stattfinden und vor allen damit die Anwendungen möglichst qualitative und homogene Metadaten aufweisen – etwa zum Zwecke der Zusammenführung und des Aufbaus übergreifender Recherchedienste – ist eine gemeinsame, fortdauernde, nachhaltige Entwicklung und Pflege von Metadatenstandards geboten.

Als ein überinstitutioneller, institutions- und projektunabhängiger Rahmen für Diskussion sowie Entwicklung und Pflege zukunftsfähiger Metadatenstandards im deutschsprachigen Raum hatte sich bereits 2013 – initiiert durch das [hbz NRW](https://www.hbz-nrw.de/) – eine OER-Metadatengruppe innerhalb des [Kompetenzzentrums Interoperable Metadaten (KIM)](https://dini.de/ag/kim/) der [Deutschen Initiative für Netzwerkinformation (DINI)](https://dini.de/) gebildet. 2017 fusionierte diese Gruppe mit der OER-Metadatengruppe von [Jointly](https://jointly.info/).

Die [Mailingliste der OER-Metadatengruppe](https://lists.dnb.de/mailman/listinfo/dini-ag-kim-oer) hat Mitglieder überwiegend aus Deutschland aber auch aus Österreich und der Schweiz. Innerhalb der Arbeitsgruppe gibt es kontinuierlichen Austausch zu den Entwicklungen im Bereich OER-Metadaten, diverse Konzepte wurden erstellt und prototypisch in der Praxis angewendet, ein [fortgeschrittener Entwurf für die strukturierte Beschreibung von OER-Diensten](https://dini-ag-kim.github.io/oer-service-card/) (Repositorien, Referatorien, Autorenwerkzeugen etc.) liegt vor.

In Anbetracht des steigenden Interesses am Thema und der wachsenden Anzahl von Menschen, die sich damit beschäftigen, soll die Arbeitsweise der Gruppe möglichst öffentlich, transparent und partizipativ gestaltet werden. Nur so kann der Anspruch gewahrt bleiben, kontinuierlich eine zentrale Anlaufstelle für alle im deutschsprachigen Raum an OER-Metadatenstandards Interessierten zu bieten.

## Werkzeuge

Im Hinblick auf die Werkzeuge werden vorzugsweise existierende Tools benutzt, die gegebenenfalls an die spezifischen Bedingungen angepasst werden.

### Spezifikationen, Standards, Empfehlungen

Dokumente mit offiziellem Charakter wie Spezifikationen, technische Standards und Empfehlungen werden als HTML/Markdown-Dokument verfasst und mit Hilfe eines speziellen DINI-Profils des [ReSpec](https://github.com/w3c/respec)-Präprozessors des W3C im Web publiziert. Die Quelldaten des Dokuments werden dabei auf [GitHub](https://github.com/dini-ag-kim) abgelegt, wo sie automatisch versioniert und mit einer nachvollziehbaren Änderungshistorie versehen werden. Zur Publikation kann zudem [GitHub Pages](https://pages.github.com/) verwendet werden, das lediglich in den Einstellungen des GitHub-Repositories aktiviert werden muss.

Durch die Verwendung von *ReSpec* können die Dokumente entweder als eine einzige Datei oder jeder Abschnitt in einer eigenen Datei gepflegt werden (siehe die untenstehenden [Beispiele](#example-specs)). *ReSpec* bereitet diese Dokumente automatisch für die Web-Publikation auf, in dem es etwa Inhaltsverzeichnisse erstellt, Querverweise einfügt, bibliografische Referenzen nachweist und Abkürzungen auflöst. Dazu müssen lediglich einige wenige Angaben zur Konfiguration von *ReSpec* gemacht werden sowie ein paar Konventionen in der Strukturierung und dem Markup eingehalten werden.

Für neue Spezifikationen kann entweder eine bestehende Spezifikation als Vorlage kopiert oder das [Blanko-Dokument](ReSpec/index.html) verwendet werden.

#### Versionierung

Für jede Spezifikation, Standard oder Empfehlung sollte ein eigenes GitHub-Repository angelegt werden. In diesem sollte sich in einem Verzeichnis `draft` die aktuelle Entwurfsfassung des Dokuments befinden, die kommentiert werden kann. Zur niedrigschwelligen Kommentierung empfiehlt es sich, den Annotationsdienst [hypothes.is](https://web.hypothes.is/) einzubinden.

Jede publizierte Version des Dokuments sollte in einem eigenen Verzeichnis abgelegt werden, das nach der jeweiligen Versionsbezeichnung benannt ist. Es empfiehlt sich, die Versionen etwa nach ihrem Veröffentlichungsdatum zu benennen (z. B. `20200131`).

Ein symbolischer Link `latest` sollte zudem immer auf die neueste publizierte Fassung verweisen. Er dient als Referenz für Verweise auf die Spezifikation, wenn dabei nicht eine konkrete Version, sondern die jeweils gültige Fassung gemeint ist.

#### <a id="example-specs"></a>Beispiele

* **Service Card for Open Educational Resources**
    * [GitHub](https://github.com/dini-ag-kim/oer-service-card)
    * [Publikation mit ReSpec](https://w3id.org/dini-ag-kim/oer-service-card/)
* **LOM for Higher Education OER Repositories**
    * [GitHub](https://github.com/dini-ag-kim/hs-oer-lom-profil)
    * [Publikation mit ReSpec](https://w3id.org/dini-ag-kim/hs-oer-lom-profil/)
* **Blanko-Vorlage für neue Spezifikationen**
    * [GitHub](https://github.com/dini-ag-kim/oer-stoeberspecs/blob/master/ReSpec/index.html)
    * [Publikation mit ReSpec](https://dini-ag-kim.github.io/oer-stoeberspecs/ReSpec/)

### Vokabulare, Ontologien

Auch Vokabulare und Ontologien werden auf [GitHub](https://github.com/dini-ag-kim) in einem eigenen Repository abgelegt und dort versioniert und gepflegt. Als Format sollte das [Simple Knowledge Organization System (SKOS)](https://www.w3.org/2004/02/skos/) verwendet werden, wobei die Kodierung idealerweise in [Turtle](https://www.w3.org/TR/turtle/)-Syntax erfolgen sollte. Die Publikation erfolgt anschließend mit [SkoHub-Vocabs](https://github.com/hbz/skohub-vocabs), einer grafischen Präsentation der Ontologie mit weitergehenden Möglichkeiten wie einer Suchfunktion (siehe [Beispiele](#example-vocab)).

#### <a id="example-vocab"></a>Beispiele

* **SKOS-Version der Destatis-Systematik der Fächergruppen, Studienbereiche und Studienfächer**
    * [GitHub](https://github.com/dini-ag-kim/hochschulfaechersystematik)
    * [Publikation mit SkoHub-Vocabs](https://w3id.org/class/hochschulfaechersystematik/scheme#)

### Kommunikation

Zur Kommunikation wird neben gelegentlichen Präsenztreffen und Videokonferenzen vor allem eine [Mailingliste](https://lists.dnb.de/mailman/listinfo/dini-ag-kim-oer) verwendet. Diese ist öffentlich und kann so von jeder/m Interessierten abonniert werden.

Die Arbeit an konkreten Spezifikationen und Standards erfolgt zusätzlich über die direkte Kommentierung der jeweiligen Entwurfsfassung (siehe oben). Diese sollte daher immer im Web publiziert werden und mit Annotationsmöglichkeiten versehen werden. Empfohlen wird neben der Verwendung der regulären GitHub-Werkzeuge wie [Issues](https://guides.github.com/features/issues/) auch die Einbindung des niedrigschwelligen Dienstes [hypothes.is](https://web.hypothes.is/).

## Organisation der Arbeitsprozesse

Vorlage für den hier beschriebenen Prozess ist der [Workflow des W3C](https://www.w3.org/2019/Process-20190301/), der jedoch aufgrund der überschaubareren Strukturen der OER-Metadatengruppe der DINI AG KIM deutlich vereinfacht wurde.

### Maintainer

Um die Pflege der Standards, Spezifikationen, Empfehlungen und Vokabulare auf GitHub zu ermöglichen, benötigt jedes Dokument mindestens einen sogenannten **Maintainer**. Diese Person oder Personengruppe verfügt über die notwendigen Berechtigungen, Änderungen am jeweiligen GitHub-Repository vorzunehmen. Außerdem obliegt ihr die Verantwortung, den Arbeitsprozess zu moderieren, d. h. etwa Fristen für die Kommentierung eines Entwurfs festzulegen, notwendige Abstimmungen durchzuführen oder bei Bedarf zusätzliche Kommunikationsmittel einzubeziehen (siehe oben).

Der oder die Maintainer entscheidet letztlich auch über den Zeitpunkt der Publikation einer neuen Version des betreffenden Dokuments, führt die entsprechenden strukturellen Änderungen im GitHub-Repository durch und verantwortet die Endredaktion.

### Pull Requests

Um die Arbeit des oder der Maintainer so einfach wie möglich zu gestalten, sollten Änderungsvorschläge nach Möglichkeit immer in Form eines [Pull Requests](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests) auf GitHub eingereicht werden. Auf diese Weise kann der Änderungsvorschlag öffentlich kommentiert, ggf. weiter verbessert und schließlich auf Knopfdruck durch den oder die Maintainer übernommen werden.

Wichtig ist, dass *Pull Requests* immer nur Änderungen an der Entwurfsfassung im Verzeichnis `draft` beinhalten, da einmal publizierte Versionen nicht mehr substantiell geändert werden sollten. Ausnahmen stellen hier nur einfache Rechtschreibfehler oder ähnliches dar, die natürlich korrigiert werden dürfen.

Alternativ können Änderungsvorschläge natürlich auch auf herkömmlichem Weg etwa per Mail an eine/n Maintainer geschickt werden, der diese dann jedoch wiederum als *Pull Request* auf GitHub dokumentieren sollte.

### Wiki

Für jedes GitHub-Repository kann in den Einstellungen ein einfaches [Wiki](https://help.github.com/en/github/building-a-strong-community/about-wikis) aktiviert werden. Dieses kann verwendet werden, um mit der Arbeit am jeweiligen Dokument in Verbindung stehende Dokumente zentral und öffentlich abzulegen (z. B. Protokolle von Videokonferenzen).

## Einführung in SKOS

* [Erste Überlegungen in CodiMD-Pad](https://pad.gwdg.de/D-QEi-z6RleT1kxBccpWww)
