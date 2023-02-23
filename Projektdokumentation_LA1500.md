# Projekt-Dokumentation

☝️ Alle Text-Stellen, welche mit einem ✍️ beginnen, können Sie löschen, sobald Sie die entsprechende Stellen ausgefüllt haben.

✍️ Ihr Gruppenname und Ihre Nachnamen

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|       | 0.0.1   | ✍️ Jedes Mal, wenn Sie an dem Projekt arbeiten, fügen Sie hier eine neue Zeile ein und beschreiben in *einem* Satz, was Sie erreicht haben. |
|       | ...     |                                                              |
|       | 1.0.0   |                                                              |

## 1 Informieren

### 1.1 Monopoly

Wir machen ein Monopoly Brettspiel.

Wir wollen ein Monopoly Brettspiel erstellen, indem man bis zu vier Leuten spielen kann. Zudem sollen auch viele Events passieren, welche zum Beispiel durch Ereigniskarten ausgelöst werden. Als ein cooles Feature wolle wir es möglich machen, dass man jegliche Felder upgraden kann, zum Beispiel das Ereignisfeld, welches dann eine erhöhte Chance für positive Effekte gibt. Das alles wollen wir mit Winforms machen, da wir gerne wieder eine visuelle Applikation machen wollen. Zudem wollen wir auch nochmal die eventbasierte Programmierung üben.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1|Spielen|Funktional| Als User möchte ich dem spiel beitreten können und mit anderen Spielern spielen. |
| 2 |Spieler|Funktional/Qualität| Als User möchte ich ein eigenes Spielfigürchen auswählen, welches mich als Spieler im Spiel repräsentiert.                          
|3| Anfangs-Betrag| Funktional| Als User möchte ich mit einem gegebenem Betrag an Geld ins Spiel starten.|  
|4|Würfel|funktional |Als User möchte ich die Anzahl Schritte welche ich gehen muss, würfeln können. |
|5| Ereignisse|Funktional|Als User möchte ich, dass das Ereignis auf welchem ich gelandet bin, passiert und ich dem nach entsprechend weiter spielen muss. |
|6 |Geldstand |Funktional/Qualität| Als User möchte ich, dass mir mein Geldstand immer angezeigt wird und aktualisiert wird wenn Abzüge oder Aufschläge stattfinden.|
|7| Kaufen| Funktional| Als User möchte ich Felder kaufen können.|
|8| Verfügbar| Funktional| Als User möchte ich sehen was zum Kauf verfügbar ist, und auch nur dann in der Lage zu sein etwas kaufen zu können. |
|9| Gebühren| Qualität| Als User möchte ich, dass die anderen Spieler mir Geld abzahlen müssen, wenn sie auf ein Feld gelangen, welches ich gekauft habe.|
|10| Sperrung| Qualität| Als User möchte ich, dass ich gesperrt werde, und nicht spielen kann, wenn ich im Gefängnis bin.|
|11| Sperrungs spezifikationen| Qualität| Als User möchte ich, dass mir angezeigt wird wieviele Runden ich noch aussetzten muss  bis ich wieder spielen darf.|
|12| Kredite | Funktional| Als User möchte Kredite bei der Bank und anderen Spielern aufnehmen können.|
|13| Verbesserungen| Rand| Als User möchte ich, was ich gekauft habe, Upgraden. Und zwar so, dass ich passives Einkommen erlange.|
verbesserungen 
✍️ Jede User Story hat eine ganzzahlige Nummer (1, 2, 3 etc.), eine Verbindlichkeit (Muss oder Kann?), und einen Typ (Funktional, Qualität, Rand). Die User Story selber hat folgende Form: *Als ein 🤷‍♂️ möchte ich 🤷‍♂️, damit 🤷‍♂️*.

### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |              |         |                   |
| ...  |              |         |                   |

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, die der Testfall abdeckt, und `m` von `1` an nach oben gezählt. Beispiel: Der dritte Testfall, der die zweite User Story abdeckt, hat also die Nummer `2.3`.

### 1.4 Diagramme

✍️Fügen Sie hier ein Use Case-Diagramm mit mindestens 10 Anwendungsfällen ein; und einen PAP.

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |       |           |              |               |
| ...  |       |           |              |               |

Total: 

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, auf die sich das Arbeitspaket bezieht, und `m` von `A` an nach oben buchstabiert. Beispiel: Das dritte Arbeitspaket, das die zweite User Story betrifft, hat also die Nummer `2.C`.

✍️ Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. Die totale Anzahl Arbeitspakete sollte etwa Folgendem entsprechen: `Anzahl R-Sitzungen` ╳ `Anzahl Gruppenmitglieder` ╳ `4`. Wenn Sie also zu dritt an einem Projekt arbeiten, für welches zwei R-Sitzungen geplant sind, sollten Sie auf `2` ╳ `3` ╳`4` = `24` Arbeitspakete kommen. Sollten Sie merken, dass Sie hier nicht genügend Arbeitspakte haben, denken Sie sich weitere "Kann"-User Stories für Kapitel 1.2 aus.

## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |       |           |               |                   |
| ...  |       |           |               |                   |

✍️ Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten.

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |              |         |                   |                      |
| ...  |              |         |                   |                      |

✍️ Verwenden Sie römische Ziffern für Ihre Bug Reports, also I, II, III, IV etc.

## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
