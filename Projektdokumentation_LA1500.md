# Projekt-Dokumentation

Petunia | Mileti, Heiniger, Hassani, Mueller

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|   23.2    | 0.0.1   |Uns für ein Spiel entschieden, Userstories erstellt, Informieren geschrieben, Use-Case und PAP Diagramme erstellt. |
|     2.3  | 0.0.2    |Weitere  5 User stories hinzugefügt, Arbeitspakete erstellt, Testfälle geschrieben.|
|       | 1.0.0   |                                                              |

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
| 3.1  |  Spieler wählt Figur aus            | Klickt auf gewünschte Figur  | Spieler spielt mit der gewünschten Figur. |
| 4.1  |  Spieler möchte anfangs Kapital            |  Spiel startet       |    1500 Spielgeld ist auf dem Konto               |
| 5.1  |  Spieler würfelt          | klicke auf den Würfelbutton        |  Spieler würfelt und geht auf das geworfene Feld.  |
| 6.1  |  Spieler steht auf einem Ereignissfeld            |  Karte wird gezogen       |   Gezogenes Event wird abgespielt.  |
| 7.1  |  Kontostand soll aktuell bleiben  |  Transaktion wird durch geführt.       | Kontostand wird upgedatet.  |
| 8.1  |  Spieler steht auf einem Feld           |  Klicke auf Kaufen       |  Feld wurde dem Käufer gutgeschrieben.|
| 9.1  |  Feld nicht Frei            |         |   Feld kann nicht gekauft werden, da es schon bei jemand anderen im Besitz ist.       |
| 10.1  |  Spieler gelangt auf fremdes Feld     | Transaktion startet.        |  Der Spieler wer dieses Feld besitzt wird Geld übertragen.|
| 11.1  | Spieler gelangt auf Gefängnisfeld             |  Zeit vergeht       | Spieler landet im Gefängniss und ist 3 Runden gesperrt.|
| 12.1  | Spieler im Gefängis             |  Runde vergeht       |  Spieler bekommt Update wie lange er noch im Gefängnis sein muss.     |
| 13.1 |  Kontostand niedrig            | Kredit anforden        |   Spieler bekommt Kredit von der Bank|
| 14.1  |  Spieler ist auf eigenem Feld             |Upgradbutton klicken         | Feld wird upgegraded und Betrag wird abgezogen |
| 15.1 |  Kontstand sehr niedrig            |  Spieler gibt Geld aus       |  Kontostand leuchtet rot auf.                 |

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, die der Testfall abdeckt, und `m` von `1` an nach oben gezählt. Beispiel: Der dritte Testfall, der die zweite User Story abdeckt, hat also die Nummer `2.3`.

### 1.4 Diagramme

![Screenshot 2023-02-23 113736](https://user-images.githubusercontent.com/111044245/220883631-c4e532a4-a307-4afe-97eb-2c4ba34fe328.png)
![Screenshot 2023-02-23 113620](https://user-images.githubusercontent.com/111044245/220883790-2752ffe2-695f-474f-8dd1-a2bd56d250f9.png)



✍️Fügen Sie hier ein Use Case-Diagramm mit mindestens 10 Anwendungsfällen ein; und einen PAP.

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |  9.3  | Lukas     | Startbutton | 25'|
| 1.B |  9.3  | Lukas     | Spielfeld | 90'|
| 3.A  |  9.3  | Ava       | Auswahl der Figuren  |  45'             |
| 3.B  |  9.3     | Ava          | Designe der Figuren   |  30' |
| 4.A  |  9.3     | Gian | Startkapital |  45'|
| 5.A  |  9.3     | Yanik    |  Würfel Button erstellen            |  20'            |
| 5.B  |  9.3     | Yanik    |  Würfel programmieren            |   45'            |
| 5.C  |  9.3     | Yanik    | Bewegung zum gewürfelten Feld    |     45'          |
| 6.A  |  9.3     | Lukas    | Ereignis Felder programmieren  |  20'             |
| 7.A  |  9.3     | Gian         | Geldstand wird upgedatet.              | 30' |
| 2.A  |  9.3     | Lukas,Gian,Ava,Yanik          |  Basic Code allen Figuren hinzufügen  | 90'              |
| 2.B  |  9.3     | Lukas,Gian,Ava,Yanik          |  Würfeln und Bewegung den Spielern Hinzufügen | 45'              |
| 2.C  |  9.3     | Lukas,Gian,Ava,Yanik          |  Erste Prototyp erstellem | 45'              |
| 6.B  |  16.3     | Lukas          | Ereignis porgrammieren    | 45'              |
| 6.C  |  16.3     | Lukas          | Ereignis wird ausgelöst | 45'               |
| 8.A  |  16.3     | Ava         | Felder Programmieren  |  70'             |
| 8.B  |  16.3     | Ava         |Preise und andere EIgenschaften hinzufügen  |  20'             |
| 8.C  |  16.3     | Ava         | Felder können gekauft werden.   |  15'            |
| 8.D  |  16.3     | Ava         | Geld wird abgezogen   |  15'            |
| 11.A  |  16.3     | Gian          |   Gefängnis Feld  |  45'             |
| 11.B  |  16.3     | Gian          |   Spieler gelant ins Gefängnis   |  45'             |
| 11.B  |  16.3     | Gian          |  Sperrung über 3 Runden + Visuell sichtbar   |  25'             |
| 13.A  |  16.3     | Yanik          | Spieler kann Kredit anfordern              |  45'             |
| 13.B  |  16.3     | Yanik          | Spieler kann Kredit zurück zahlen            |  20'             |
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
