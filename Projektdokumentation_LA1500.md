# Projekt-Dokumentation

Petunia | Mileti, Heiniger, Hassani, Mueller

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|   23.2    | 0.0.1   |Uns für ein Spiel entschieden, Userstories erstellt, Informieren geschrieben, Use-Case und PAP Diagramme erstellt. |
|   2.3     | 0.0.2    |Würfel und Spielbrett wurden angefangen.|
|   9.3     | 0.0.3   | Spielfigur kann sich bewegen.  |
|  29.3     | 1.0.0   | Prototyp fertig  |

## 1 Informieren

### 1.1 Monopoly

Wir machen ein Monopoly Brettspiel.

Wir wollen ein Monopoly Brettspiel erstellen, indem man bis zu vier Leuten spielen kann. Zudem sollen auch viele Events passieren, welche zum Beispiel durch Ereigniskarten ausgelöst werden. Als ein cooles Feature wolle wir es möglich machen, dass man jegliche Felder upgraden kann, zum Beispiel das Ereignisfeld, welches dann eine erhöhte Chance für positive Effekte gibt. Das alles wollen wir mit Winforms machen, da wir gerne wieder eine visuelle Applikation machen wollen. Zudem wollen wir auch nochmal die eventbasierte Programmierung üben.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1|muss|Funktional| Als User möchte ich dem spiel beitreten können und mit anderen Spielern spielen. |
|2| muss| Funktional| Als User möchte ich, dass weitere drei User dem Spiel beitreten können, damit diese mit mir spielen können. |
| 3 |kann|Funktional/Qualität| Als User möchte ich ein eigenes Spielfigürchen auswählen, damit dieses mich als Spieler im Spiel repräsentiert.|       
|4|muss| Funktional| Als User möchte ich mit einem gegebenem Betrag an Geld ins Spiel starten, damit das Spiel ins Rollen kommt.|  
|5|muss|Funktional |Als User möchte ich die Anzahl Schritte welche ich gehen muss, würfeln können, damit ein gewisser Grad an Zufall mitspielt. |
|6| kann|Funktional|Als User möchte ich, dass das Ereignis auf welchem ich gelandet bin, passiert und ich dem nach entsprechend weiter spielen muss. |
|7 |muss|Funktional/Qualität| Als User möchte ich, dass mir mein Geldstand immer angezeigt wird und aktualisiert wird wenn Abzüge oder Aufschläge stattfinden, damit ich auf neuestem Stand bin und dem nach Handeln kann.|
|8|muss| Funktional| Als User möchte ich Felder kaufen können, damit ich anderen voraus bin.|
|9| muss| Funktional| Als User möchte ich sehen was zum Kauf verfügbar ist, und auch nur dann in der Lage zu sein etwas kaufen zu können, damit ich weiss was verfügbar ist und was nicht. |
|10|muss| Qualität| Als User möchte ich, dass die anderen Spieler mir Geld abzahlen müssen, wenn sie auf ein Feld gelangen, welches ich gekauft habe, damit ich Umsatz mache von den was ich gekauft habe.|
|11|kann| Qualität| Als User möchte ich, dass ich gesperrt werde, wenn ich im Gefängnis bin, damit ich auf keine Weise weiter Spielen kann.|
|12|kann| Qualität| Als User möchte ich, dass mir angezeigt wird wieviele Runden ich noch aussetzten muss  bis ich wieder spielen darf, damit ich mir dem Bewusst bin und wieder spielen kann.|
|13|kann| Qualität| Als User möchte Kredite bei der Bank und anderen Spielern aufnehmen können.|
|14|kann| Rand| Als User möchte ich, was ich gekauft habe, Upgraden. Und zwar so, dass ich passives Einkommen erlange.|
|15| kann| Qualität| Als User möchte ich, dass wenn mein Kontostand zu niedrig wird, dieser in Rot aufleuchtet, damit ich ihn sehe.|
|16| kann| Funktional| Als User möchte ich, dass man seine Felder tauschen kann, damit das Spiel spannender wird.|
|17| kann| Rand| Als User möchte ich den Spielstand abspeichern, damit ich später weiter spielen kann.|
|18| kann| Rand| Als Spieler möchte ich aufgeben können, damit ich aufhören kann. |
|19| kann| Rand| Als Spieler möchte ich einen Timer, damit man sehen kann wie lange man schon spielt.|

### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe|
| ---- | ------------ | ------- | ----------------- |
| 1.1  |  Spieler will spielem |  Klickt den Startbutton       |  Spielstartet|
| 2.1  |  Spieler wählt Figur aus            | Klickt auf gewünschte Figur  | Spieler spielt mit der gewünschten Figur. |
| 3.1  |  Spieler möchte anfangs Kapital            |  Spiel startet       |    1500 Spielgeld ist auf dem Konto               |
| 4.1  |  Spieler würfelt          | klicke auf den Würfelbutton        |  Spieler würfelt und geht auf das geworfene Feld.  |
| 5.1  |  Spieler steht auf einem Ereignissfeld            |  Karte wird gezogen       |   Gezogenes Event wird abgespielt.  |
| 6.1  |  Kontostand soll aktuell bleiben  |  Transaktion wird durch geführt.       | Kontostand wird upgedatet.  |
| 7.1  |  Spieler steht auf einem Feld           |  Klicke auf Kaufen       |  Feld wurde dem Käufer gutgeschrieben.|
| 8.1  |  Feld nicht Frei            |         |   Feld kann nicht gekauft werden, da es schon bei jemand anderen im Besitz ist.       |
| 9.1  |  Spieler gelangt auf fremdes Feld     | Transaktion startet.        |  Der Spieler wer dieses Feld besitzt wird Geld übertragen.|
| 10.1  | Spieler gelangt auf Gefängnisfeld             |  Zeit vergeht       | Spieler landet im Gefängniss und ist 3 Runden gesperrt.|
| 11.1  | Spieler im Gefängis             |  Runde vergeht       |  Spieler bekommt Update wie lange er noch im Gefängnis sein muss.     |
| 12.1 |  Kontostand niedrig            | Kredit anforden        |   Spieler bekommt Kredit von der Bank|
| 13.1  |  Spieler ist auf eigenem Feld             |Upgradbutton klicken         | Feld wird upgegraded und Betrag wird abgezogen |
| 14.1 |  Kontstand sehr niedrig            |  Spieler gibt Geld aus       |  Kontostand leuchtet rot auf.                 |
| 15.1 |  Spieler möchte nicht mehr spielen            |  Spieler klickt auf Aufgeben       |  Spiel wird geschlossen.              |
| 16.1 |  Spieler geht über LOS           |  Spieler bekommt 200 Dollar       |  Kontostand wir um 200 erhöht.                  |





### 1.4 Diagramme

![Screenshot 2023-02-23 113736](https://user-images.githubusercontent.com/111044245/220883631-c4e532a4-a307-4afe-97eb-2c4ba34fe328.png)
![Use-Case-Diagramm drawio](https://user-images.githubusercontent.com/89087859/230322797-967831b2-0540-490e-8e37-1b74288c11bf.png)




## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |  9.3  | Lukas     | Startbutton und Menu | 25'|
| 1.B |  9.3  | Lukas     | Spielfeld | 90'|
| 3.A  |  9.3  | Ava       | Auswahl der Figuren  |  45'             |
| 3.B  |  9.3     | Ava          | Designen der Figuren   |  30' |
| 4.A  |  9.3     | Gian | Startkapital |  45'|
| 5.A  |  9.3     | ürsprünglich Yanik, gemacht: Gian    |  Würfel Button erstellen            |  20'            |
| 5.B  |  9.3     | ürsprünglich Yanik, gemacht: Gian    |  Würfel programmieren            |   45'            |
| 5.C  |  9.3     | ürsprünglich Yanik, angefangen Ava Lukas   | Bewegung zum gewürfelten Feld    |     45'          |
| 6.A  |  9.3     | Lukas    | Ereignis Felder programmieren  |  20'             |
| 7.A  |  9.3     | Gian         | Geldstand wird upgedatet.              | 30' |
| 2.A  |  9.3     | Gian          |  Basic Code allen Figuren hinzufügen  | 45'              |
| 2.B  |  9.3     | ürsprünglich Yanik, gemacht Lukas      |  Würfeln und Bewegung den Spielern Hinzufügen | 45'              |
| 2.C  |  9.3     | Lukas         |  Erste Prototyp erstellem | 45'              |
| 6.B  |  16.3     | Lukas          | Ereignis porgrammieren    | 45'              |
| 6.C  |  16.3     | Lukas          | Ereignis wird ausgelöst | 45'               |
| 8.A  |  16.3     | Ava         | Felder Programmieren  |  70'             |
| 8.B  |  16.3     | Ava         |Preise und andere EIgenschaften hinzufügen  |  20'             |
| 8.C  |  16.3     | Ava         | Felder können gekauft werden.   |  15'            |
| 8.D  |  16.3     | Ava         | Geld wird abgezogen   |  15'            |
| 11.A  |  16.3     | Gian          |   Gefängnis Feld  |  45'             |
| 11.B  |  16.3     | Gian          |   Spieler gelangt ins Gefängnis   |  45'             |
| 11.B  |  16.3     | Gian          |  Sperrung über 3 Runden + Visuell sichtbar   |  25'             |
| 13.A  |  16.3     | ürsprünglich Yanik, gemacht Lukas           | Spieler kann Kredit anfordern              |  45'             |
| 13.B  |  16.3     | ürsprünglich Yanik, gemacht Lukas          | Spieler kann Kredit zurück zahlen            |  20'             |
| 15.A  |  16.3     | Yanik          | Kontostand leuchtet rot auf wenn er sehr niedrig ist. |    45'           |
| 14.A  |  16.3     |  Lukas         | Upgrade von Ereignisfelder            | 45'              |
| 14.A  |  23.3     |  Yanik         | Abzug der Miete wenn man auf fremdem Feld ist             |     45'          |
| 12.A  |  23.3      |  Lukas        | Runden erstellen             |  45'             |
| 16.A  |  23.3      |  Gian         | Handelmenu erstellen   |    45'           |
| 16.B  |  23.3      |  Gian        |  Handel Funktion fertigstellen            | 45'              |
| 17.A  |  23.3      | Yanik          |  Spielstand abspeicher            |  45'             |
| 17.B  |  23.3      | Yanik         |  Spielstand laden            |  45'             |
| 18.A  |  23.3      | Ava          |  Aufgeben Button erstellen            |       15'        |
| 18.B |  23.3      | Ava          |  Aufgeben Button programmieren          |  45'             |
| 19.A  |  23.3     |  Lukas         |    Timer erstellen          |   30'            |
| 19.B  |  23.3     |  Lukas         |    Timer programmieren         |   45'            |


Total: 35 Arbeitspackete



## 3 Entscheiden

Zuerst wollten wir ein 4 Spieler Monopoly machen, jedoch reichte die Motivation in der Gruppe wie auch die Zeit nicht aus, um ein 4 Spieler Monopoly zu machen
deswegen haben wir uns entschieden, einen Prototyp zu erstellen, welcher nur von einer Person bespielt werden kann.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.B  | 09.03.2023 | Lukas          |   90'            |   90'  |
| 5.A  | 09.03.2023      | Gian          |  20'             |     5' |
| 5.B  | 09.03.2023      | Gian          |   45'            |    30'               |
| 5.C  | 09.03.2023      | Lukas und Ava  |  45'             |   120' noch nicht fertig  |
| 1.A  | 09.03.2023     | Gian          |   25'            |     55' noch nicht Fertig              |
| 5.C  | 16.03.2023      | Lukas und Ava  |  45'             |   120' fertig  |
| 6.A | 16.03.2023       |  Lukas         |  45'             |   60' angefangen                |
| 2.B  | 16.03.2023 | Lukas          |   90'            |   90'  |
| 17.A |16.03.2023 |Gian |    90'    |     90' angefangen |
| 2.C  | 09.03.2023 | Lukas          |   90'            |   90'  |
| 11.A  | 29.03.2023 | Lukas          |   45'            |   20'  |
| 11.B | 29.03.2023 | Lukas          |   45'            |   20'  |
| 13.A | 29.03.2023 | Lukas          |   45'            |   10'  |
| 13.B | 29.03.2023 | Lukas          |   20'            |   10'  |
| 18.A | 29.03.2023 | Lukas          |   15'            |   10'  |
| 18.B | 29.03.2023 | Lukas          |   45'            |   10'  |
| 19.A | 29.03.2023 | Lukas          |   35'            |   20'  |
| 19.B | 29.03.2023 | Lukas          |   45'            |   20'  |
| 19.B | 29.03.2023 | Lukas          |   20'            |   14'  |



## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 06.04.2023 |  negativ  | Lukas       |
| 2.1  | 06.04.2023 |  negativ         |Lukas        |
| 3.1  | 06.04.2023 |  negativ        | Lukas       |
| 4.1  | 06.04.2023 |  positiv       | Lukas       |
| 5.1  | 06.04.2023 |  positiv        | Lukas       |
| 6.1  | 06.04.2023 |  positiv        | Lukas       |
| 7.1  | 06.04.2023 |  negativ        | Lukas       |
| 8.1  | 06.04.2023 |  negativ        | Lukas       |
| 9.1  | 06.04.2023 |  negativ        | Lukas       |
| 10.1  | 06.04.2023 |  positiv      | Lukas       |
| 11.1  | 06.04.2023 |  negativ        | Lukas       |
| 12.1  | 06.04.2023 |  positiv        | Lukas       |
| 13.1  | 06.04.2023 |  negativ        | Lukas       |
| 14.1  | 06.04.2023 |  negativ        | Lukas       |
| 15.1  | 06.04.2023 |  positiv        | Lukas       |
| 16.1  | 06.04.2023 |  positiv        | Lukas       |


Das Spiel ist in diesem Zustand eher ein Rohling als ein fertiges Spiel, dennoch würde ich sagen sind die Ansätze von Monopoly gegeben sind.
Trotzdem finde ich, könnte man aus diesem Rohling noch ein super tolles Spiel machen. Aber leider übermannen die negativen Resultate die Positive, deswegen würde ich
sage, dass das Spiel nicht wirklich spielbar ist.





## 6 Auswerten

(https://github.com/Gian099/LA1500/blob/main/Lernbericht.md)
