# Auftrag 1
 Erstellen sie eine leere Tabelle mit 6 Kolonnen und 16 Zeilen. Füllen sie diese wie 
folgt aus:
1. Kolonne: Dezimalzahlen von 0 bis 15
2. Kolonne: Hexadezimalzahlen von 0 bis F
3. Kolonne, 4. Kolonne, 5. Kolonne und 6. Kolonne die entsprechenden Binärzahlen
Studieren sie nun ihre fertig ausgefüllte Tabelle, insbesondere die Kolonnen mit den 
Binärwerten. Was stellen sie fest?

**Feststellung**<br>
In der binären Darstellung von Zahlen wird die Frequenz der Symbole 0 und 1 mit jedem zusätzlichen Bit verdoppelt. Jedes Bit repräsentiert einen Platzwert, und mit jedem weiteren Bit erhöht sich die Anzahl der möglichen Kombinationen um das Doppelte. Das bedeutet, dass die binäre Frequenz mit jedem Bit halbiert wird, wodurch die Vielfalt der darstellbaren Werte exponentiell zunimmt. In der vorliegenden Tabelle illustrierst du diesen Prozess anschaulich von 0 bis 15, wobei jedes Bit die Anzahl der möglichen Zustände verdoppelt.

| DEZ | HEX | BIN  |
|-----|-----|------|
| 0   | 0   | 0000 |
| 1   | 1   | 0001 |
| 2   | 2   | 0010 |
| 3   | 3   | 0011 |
| 4   | 4   | 0100 |
| 5   | 5   | 0101 |
| 6   | 6   | 0110 |
| 7   | 7   | 0111 |
| 8   | 8   | 1000 |
| 9   | 9   | 1001 |
| 10  | A   | 1010 |
| 11  | B   | 1011 |
| 12  | C   | 1100 |
| 13  | D   | 1101 |
| 14  | E   | 1110 |
| 15  | F   | 1111 |

# Auftrag 2
Wandeln sie die folgende Dezimalzahl ohne Taschenrechner in die entsprechende 
Binärzahl um: ``911``

| DEZ | HEX | BIN  |
|-----|-----|------|
| 9   | 9   | 1001 |
| 1   | 1   | 0001 |
| 1   | 1   | 0001 |

**Antwort:**<br>
Wenn man die Zahl ``911`` in eine Binärzahl umwandelt bekommt man folgendes: 
``1001 0001 0001`` 

# Auftrag 3
Wandeln sie die folgende Binärzahl ohne Taschenrechner in die entsprechende 
Dezimalzahl um: ``1011'0110``

**Lösungsweg:**<br>
Um diese Zahl in eine Dezimalzahl umzuwandeln müssen wir zuerst alle bits und ihre Werte einzeln aufschreiben:

| VAL | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|-----|-----|----|----|----|---|---|---|---|
| BIN | 1   | 0  | 1  | 1  | 0 | 1 | 1 | 0 |

Also wenn wir diese zahlen alle zusammenzahlen bekommen wir die Zahl: 
``182``

# Auftrag 4
Wandeln sie die folgende Binärzahl ohne Taschenrechner in die entsprechende 
Hexadezimalzahl um: ``1110'0010'1010'0101``

**Lösungsweg:**<br>
Ich habe die Binärzahl in vier 4er-Gruppen aufgeteilt. Diese habe ich dann in ``DEZ`` umgewandelt, sodass es einfacher ist es in `HEX` umzuwandeln. Wenn man oben bei Auftrag 1 nachschaut kann man sehen welche `DEZ` Werte auf `HEX` Werte zutreffen.

| BIN | 1110 | 0010 | 1010 | 0101 |
|-----|------|------|------|------|
| DEZ | 14   | 2    | 10   | 5    |
| HEX | E    | 2    | A    | 5    |

# Auftrag 5
Was ergibt die Addition der beiden binären Zahlen ``1101'1001`` und ``0111'0101``? 
Beachten sie, dass für das Resultat ebenfalls nur 8 Binärstellen zur Verfügung 
stehen. 

**Lösungsweg:**<br>
Um die beiden binären Zahlen `11011001` und `01110101` zu addieren, können Sie die übliche Addition von rechts nach links durchführen, wobei Sie den Übertrag von einer Stelle zur nächsten berücksichtigen. Hier ist der Rechenweg:

```
   1101'1001   
 + 0111'0101
  __________
  1 0100'1110   
```

Das Ergebnis der Addition ist `01001110`. Beachten Sie, dass ich den Übertrag am Anfang hinzugefügt habe, um sicherzustellen, dass alle Stellen korrekt addiert werden. Da nur 8 Binärstellen erlaubt sind, wird das Ergebnis auf die ersten 8 Stellen beschränkt, und der Übertrag wird ignoriert. Daher ist das Endergebnis `01001110`.


