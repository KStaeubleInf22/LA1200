# Projekt-Dokumentation

Coyote
Noah Meier, Simon Frey, Benas Sivickas und Kilian Stäuble

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|27.10.2022| 0.1   | Wir haben ein wenig Brainstorming getätigt und die Projektdokumenation nach IPE geschrieben.|
| 03.11.2022|0.2   | Wir haben begonnen mit dem Programmieren des Programmes ausserdem wurde die Projektdokumentation noch angepasst.|
|10.11.2022| 0.3| Wir Haben den Code bearbeitet und die Projektdokumentation bearbeitet.|
|17.11.2022| 0.4| Die Proketdokumentation wurde fertiggeschrieben und
## 1 Informieren

### 1.1 Ihr Projekt

WIr werden eine Konsolenapplikation erstellen, die Benutzer zu Gruppen zuteilen kann nach 3 gesetzten Prioritäten, die der Benutzer zuvor eingegeben hat und dann möglichst gerecht darin eingeteilt werden.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    | muss                | Funktional | Als ein Benutzer möche ich eine Datei schreiben können, welcher Alle Daten (Alle Teilnehmer, Mailadadresse und Workshops nach Prioritäten von vorne nach hinten sortiert) drinn stehen, aus welcher die Daten ausgelesen werden.
| 2  | muss                 |Funktional| Als ein Benutzer möchte ich eine Datei mit drei Workshops eingeben können, damit das Programm mich in einer dieser Kurse einteilen kann.|
| 3  | muss            |Qualität| Als ein Benutzer möchte ich Prioritäten für die Workshops setzten, damit das Programm best möglich alle Teilnehmer in einen Workshop einteilen kann.|
| 4  | muss          |Funktional| Als ein Benutzer möchte ich, dass das Programm mich möglichst in einen Workshop zuteilt, den ich auch besuchen möchte.|
| 5  | kann         | Funktional     | Als ein Benutzer möchte ich, dass das Programm mit Try Catch arbeiten kann, damit er eine Rückmeldung erhält, falls eine falsche eingabe gemacht wurde.|
| 6  |muss                |Qualität| Als Benutzer möchte ich nicht weniger als 4 Personen und nicht mehr als 20 in dem selben Workshop haben.|



### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |   Programm wurde gestartet| Datei | Danke für die Datei.|
| 1.2 |   1.1 | Keine | Teilnehmer Nummer und Mailadresse.|
| 2.1  |     1.1      |  Keine| Priorität 1: Workshop   |
| 2.2  |     2.1  Workshop 1 wurde korrekt erkannt. |   Keine |  Priorität 2: Wokrshop       |
| 2.3  |     2.2 Workshop 2 wurde korrekt erkannt.       |  Datei   |  Priorität 3: Workshop              |
| 3.1  |     1.1   |Keine| Korrektes auslesen und zuordnen der Prioritäten.|
| 4.1  |     Alle Teilnehmer wurden aus der Datei erfasst. Keine | Workshops mit all den Teilnehmern nach Prioritäten eingeteilt, bis Sie voll sind.|
| 5.1 |     Datei wird gelesen   |  Keine       |   Fehler, Bitte überprüfe die Datei nochmals nach Fehlern.|
| 6.1 |     Datei wird gelesen, 4.1| Keine | Korrekte Anzahl der Teilnehmer wird jedem Workshop zugeteilt.|

### 1.4 Diagramme

✍️ Hier können Sie PAPs, Use Case- und Gantt-Diagramme oder Ähnliches einfügen.

## 2 Planen



| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 03.11.2022 |    Benas + Noah       |Datei kann in die Konsolenapplikation ausgelesen/übersetzt werden.| 3x45min
| 2.A | 03.11.2022 |       Benas    | Nur das Ausgeben wird programmiert mit Variabeln und später mit den richtigen ersetzt.| 45min|
|3.A  | 10.11.2022 |     Benas      | Zuordnen der Prioritäten aus der Datei.| 45min|
| 4.A  | 10.11.2022 |    Benas       |Analysieren der Anzahl Teilnehmer in den Workshops.| 45min|
| 5.A  | 10.11.2022 |    Benas       | Fehlererkennung aus der Datei.| 45min|
| 6.A  | 10.11.2022 |     Benas      | Zählung der Teilnehmer in Workshops und weiteres verteilen, falls zu wenig oder zuviel schon in einem Workshop sind.| 45min|



## 3 Entscheiden

Wir entschieden uns für eine Fehlererkennung falls ein Workshop falsch geschrieben wurde, dass dieser übersprungen wird und als keine Daten zählt.
## 4 Realisieren


| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  | 03.11.2022 | Benas + Noah        | 3x45min              |  3x45min                 |
| 2.A | 03.11.2022 |   Benas        | 45min | 45min|
|3.A  | 10.11.2022 |   Benas        | 45min | 30min|
| 4.A  | 10.11.2022 |  Benas         |45min| 60min|
| 5.A  | 10.11.2022 |    Benas       | 45min| 45min|
| 5.A  | 10.11.2022 |    Benas       | 45min| 45min|


## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 3.11      | Ok        | Benas |
| 1.2  | 3.11      | Ok         | Benas       |
| 2.1  | 3.11      | Ok         | Benas       |
| 2.2  | 10.11      | Ok         | Kilian       |
| 2.3  | 10.11      | Ok         | Noah       |
| 3.1  | 17.11      | Ok         | Kilian       |
| 4.1  | 17.11      | Nicht Ok    |        |
| 5.1  | 17.11      | Nicht Ok   |        |
| 6.1  | 17.11      | Nicht Ok |        |





## 6 Auswerten
https://github.com/KStaeubleInf22/LA1200/blob/main/Lernbericht.md
