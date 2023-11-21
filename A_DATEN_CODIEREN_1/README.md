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

# Auftrag 6
Was könnten die beiden folgenden binären Wert für eine Bedeutung haben?
(Tipp: a. ins Dezimalsystem umrechnen, b. ins Hexadezimalsystem umrechnen)

a.`` 1100 0000 . 1010 1000 . 0100 1100 . 1101 0011``

b. ``1011 1110 - 1000 0011 - 1000 0101 - 1101 0101 - 1110 0100 - 1111 1110``

**Lösungsweg:**<br>
**a)**<br>
Die Antwort hier ist eigentlich sehr einfach es ist eine `IP-Adresse`. Ich bin folgend auf diese Antwort gekommen.

1. Es sind 4 Oktette, die durch punkte seperiert werden.
2. Wenn man das erste Oktett(links) in eine Dezimalzahl umwandelt ergibt diese `192`

**b)**<br>
Die Antwort hier ist ebenfalls ziemlich einfach, da diese 6 Binär Oktetten auf eine MAC-Adresse hinweisen, da es niemals eine IPv6 Adresse sein könnte, da diese 16-Oktette hat mit einer gesamt zahl von 128bits.

**Antwort Auftrag 6 a:**

Wenn man die 4 Binär Oktette `` 1100 0000 . 1010 1000 . 0100 1100 . 1101 0011`` in Dezimalzahlen umwandelt erhält man folgende IPv4 Adresse: `192.176.76.211`

**Antwort Auftrag 6 b:**

Um die binäre Zahl in Hexadezimal umzuwandeln, gruppiere die Binärziffern in Gruppen von 4 Bits und wandele jede Gruppe in ihre entsprechende hexadezimale Darstellung um:

```
1011 1110 - 1000 0011 - 1000 0101 - 1101 0101 - 1110 0100 - 1111 1110
```

Die Hexadezimaldarstellung jeder Gruppe:

```
BE - 83 - 85 - D5 - E4 - FE
```

Also ist die Hexadezimaldarstellung der gegebenen binären Zahl: `BE-83-85-D5-E4-FE`.

# Auftrag 7
Für Linux-Fans: Was könnte die folgende in einem Bash-Script entdeckte Zeile für 
eine Bedeutung haben? ``chmod 751 CreateWeeklyReport``

**Lösungsweg:**

Die Zeile `chmod 751 CreateWeeklyReport` in einem Bash-Script hat die Bedeutung, dass die Berechtigungen (permissions) für die Datei oder das ausführbare Programm namens "CreateWeeklyReport" gesetzt werden.

1. **`chmod`**: Dieser Befehl wird verwendet, um die Zugriffsrechte auf Dateien zu ändern.

2. **`751`**: Dies ist der Teil, der die Berechtigungen festlegt. In Linux werden die Berechtigungen in drei Gruppen unterteilt: Besitzer (owner), Gruppe (group) und andere (others). Die Ziffern 7, 5 und 1 repräsentieren die Berechtigungen für den Besitzer, die Gruppe und andere.

   - **7**: Das ist die Summe der Berechtigungen `rwx` (Lesen, Schreiben, Ausführen).
   - **5**: Das ist die Summe der Berechtigungen `r-x` (Lesen, Nicht Schreiben, Ausführen).
   - **1**: Das ist die Summe der Berechtigungen `--x` (Nicht Lesen, Nicht Schreiben, Ausführen).

   Zusammen bedeutet dies, dass der Besitzer volle Berechtigungen hat (`rwx`), die Gruppe nur Lese- und Ausführungsrechte (`r-x`) hat, und andere nur Ausführungsrechte (`--x`) haben.

3. **`CreateWeeklyReport`**: Dies ist der Name der Datei oder des ausführbaren Programms, für das die Berechtigungen geändert werden.

Zusammengefasst bedeutet die Zeile also, dass der Besitzer die volle Kontrolle über die Datei hat, die Gruppe Lese- und Ausführungsrechte hat, und andere nur Ausführungsrechte haben. Dies könnte beispielsweise in einem Szenario verwendet werden, in dem der Besitzer die Datei erstellen und ausführen kann, die Gruppe sie nur ausführen kann, und andere Benutzer sie ebenfalls nur ausführen können.

# Auftrag 8:
Dimensionieren sie für den Matterhorn-Express, wo insgesamt 107 Gondeln die 
Touristen von Zermatt auf den Trockenen-Steg befördern, die Codebreite des 
Binärcodes für die Kabinenzählung.

**Lösungsweg:**

Wenn man die Codebreite bzw. die anzahl der Bits für 107 Gondeln bzw. der Wert 107 berechnen möchte muss man zuerst wissen welche Bits aktiviert werden müssen um die Zahl 107 darzustellen. Hierzu schauen wir die Bits tabelle an:

| 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|----|----|----|---|---|---|---|

Die Maximale Anzahl werte die man mit `7-Bits` anzeigen kann ist 127 oder 128(mit 0 inkl.) Das heisst hier braucht man maximal `7-Bits` um die Zahl 107 darzustellen.

# Auftrag 9:
 Sie untersuchen einen Arbeitsspeicher mit 12-Bit-Adress- bzw. 16-Bit-Datenbus.
Welche Speicherkapazität in kiB besitzt dieser? (Hinweis: 1kiB=1024B)

**Lösungsweg:**

Um die Speicherkapazität in KiB zu berechnen, multiplizieren Sie die Anzahl der Adressen mit der Größe der Daten und teilen durch 1024:

\[ Speicherkapazität_{KiB} = \frac{4096 \times 65536}{1024} \]

\[ Speicherkapazität_{KiB} = \frac{268435456}{1024} \]

\[ Speicherkapazität_{KiB} = 262144 \, KiB \]

Also hat der Arbeitsspeicher mit einem 12-Bit-Adressbus und einem 16-Bit-Datenbus eine Kapazität von 262144 KiB.

# Auftrag 10:
Zwei Geräte sind mit einer seriellen Leitung und zusätzlichem Taktsignal verbunden. 
Das Taktsignal beträgt 1MHz.
a. Wie viele Bytes können damit pro Sekunde übertragen werden?
b. Wie viele Bytes pro Sekunde könnten übertragen werden, wenn die 
Verbindung der beiden Geräte nicht seriell, sondern 8 Bit-parallel wäre?

**Lösungsweg:**

a. Serielle Übertragung:
Die Übertragungsgeschwindigkeit (Datenrate) bei serieller Übertragung wird durch das Taktsignal bestimmt. Da es sich um eine serielle Verbindung handelt, wird jedes Bit separat übertragen. Die Formel für die Datenrate lautet:

\[ \text{Datenrate} = \text{Taktfrequenz} \times \text{Anzahl der Bits pro Übertragung} \]

In diesem Fall beträgt die Taktfrequenz 1 MHz und die Übertragung erfolgt seriell, was bedeutet, dass nur 1 Bit pro Übertragung übertragen wird.

\[ \text{Datenrate} = 1 \, \text{MHz} \times 1 \, \text{Bit} = 1 \, \text{Mbps} \]

Um die Anzahl der Bytes pro Sekunde zu berechnen, teilen Sie die Datenrate durch 8 (da 1 Byte = 8 Bits):

\[ \text{Bytes pro Sekunde} = \frac{\text{Datenrate}}{8} = \frac{1 \, \text{Mbps}}{8} = 125 \, \text{kBps} \]

b. 8 Bit-parallele Übertragung:
Bei paralleler Übertragung werden mehrere Bits gleichzeitig übertragen. In diesem Fall beträgt die Breite der parallelen Übertragung 8 Bit.

Die Datenrate bei paralleler Übertragung wird durch die Formel bestimmt:

\[ \text{Datenrate} = \text{Taktfrequenz} \times \text{Anzahl der Bits pro paralleler Übertragung} \]

Hier beträgt die Taktfrequenz 1 MHz und die Anzahl der Bits pro paralleler Übertragung 8 Bit.

\[ \text{Datenrate} = 1 \, \text{MHz} \times 8 \, \text{Bit} = 8 \, \text{Mbps} \]

Um die Anzahl der Bytes pro Sekunde zu berechnen, teilen Sie die Datenrate durch 8:

\[ \text{Bytes pro Sekunde} = \frac{\text{Datenrate}}{8} = \frac{8 \, \text{Mbps}}{8} = 1 \, \text{MBps} \]

Zusammengefasst: Bei serieller Übertragung beträgt die Datenrate 1 Mbps, was 125 kBps entspricht. Bei paralleler Übertragung beträgt die Datenrate 8 Mbps, was 1 MBps entspricht.

# Auftrag 11
 Bei den bisherigen Aufgaben zu Binärcodes, handelte es sich immer um positive, 
numerische Werte. Bei den Programmiersprachen spricht man vom Datentyp 
"unsigned integer". Hin und wieder möchte man aber auch die negative Zahlenwelt 
miteinbeziehen, man nennt dies dann "signed integer", was mit vorzeichenbehaftete 
Ganzzahl übersetzt werden kann.

(*Wobei man gut beraten ist, abzuwägen, ob der Mehraufwand für negative Zahlen tatsächlich 
gerechtfertigt ist, wie folgendes Beispiel aus der Physik zeigt: Die Celsius-Temperaturskala kennt 
negative Werte, die Kelvin-Temperaturskala hingegen nicht und beide Skalen messen dieselbe 
Temperatur. Zum Beispiel entspricht der absolute Temperatur-Nullpunkt (nichts kann kälter sein, dass ist 
in diesem Fall entscheidend) -273 Grad Celsius aber eben auch 0 Grad Kelvin, Wasser schmilzt bei 0 
Grad Celsius bzw. 273 Grad Kelvin und der heutige Sommer bot angenehme 35 Grad Celsius oder eben 
308 Grad Kelvin*)

Möchte man den binären Zahlenstrahl in den negativen Bereich erweitern, liegt die 
Versuchung nahe, das erste Bit (MSB) als Vorzeichen zu verwenden. Funktioniert 
leider nicht bzw. nicht in allen Fällen! Die Lösung die funktioniert, nennt man 
Zweierkomplement. Was darunter zu verstehen ist, wird im Internet unzählige Male 
erklärt.
Nun zur Aufgabe: Wir gehen von einer Verarbeitungsbreite von einem Byte aus. 
(Datenbusbreite:1Byte)

**Lösungsweg:**

**a. Unsigned Integer (Vorzeichenlos):**

   Der kleinste Binärwert mit einem Byte ist 00000000, was im Dezimalsystem 0 entspricht.
   
   Der größte Binärwert mit einem Byte ist 11111111, was im Dezimalsystem 255 entspricht.

**b. Signed Integer (Vorzeichenbehaftet):**

   Da wir von einem Byte ausgehen, verwendet man das erste Bit (Most Significant Bit - MSB) als Vorzeichenbit bei signed Integern. Für ein Byte:

   Der kleinste Binärwert ist 10000000, was im Dezimalsystem -128 entspricht.

   Der größte Binärwert ist 01111111, was im Dezimalsystem 127 entspricht.

**c. Dezimalzahl +83 in vorzeichenbehafteten Binärwert umwandeln (signed):**

   Dezimal +83 ist im Binärsystem 01010011.

**d. Dezimalzahl -83 in vorzeichenbehafteten Binärwert umwandeln (signed):**

   Dezimal -83 wird im Zweierkomplement umgewandelt. Zuerst wird die Binärdarstellung von +83 genommen (01010011) und dann jedes Bit invertiert (10101100), und anschließend wird 1 addiert: 10101100 + 1 = 10101101.

**e. Addition der beiden Binärwerte:**

   \(01010011 + 10101101 = 0\) (Beachte: Dies ist im Zweierkomplement)

**f. Dezimalzahl 0 in vorzeichenbehafteten Binärwert umwandeln (signed):**

   Dezimal 0 bleibt im Binärsystem 00000000.

   Die vorangegangene Addition ergab in der Tat 0, da \(01010011 + 10101101 = 0\) im Zweierkomplement.

**g. Warum kann die Dezimalzahl +150 nicht in einen vorzeichenbehafteten Binärwert umgewandelt werden?**

   Bei einem Byte und signed Integer reicht der Wertebereich nur von -128 bis 127. Die Zahl +150 liegt außerhalb dieses Bereichs und kann daher nicht in einen vorzeichenbehafteten Binärwert umgewandelt werden. Dies verdeutlicht die Begrenzungen des Wertebereichs, wenn man signed Integers verwendet.

# Auftrag 12

Bisher haben wir immer von ganzen Zahlen gesprochen. Oft genügt das in der realen 
Welt aber nicht. Dazu ein Beispiel: Teile ich die Ganzzahl 1 durch die Ganzzahl 3 und 
multipliziere sie darauf wieder mit der Ganzzahl 3 erhalte ich, sofern der 
Compiler/Interpreter nicht trickst, die Ganzzahl 0, was bekanntlich falsch ist. Dies weil 
das Resultat der Division nicht als 0.3333333 sondern als ganze Zahl 0 
(Nachkommastellen werden ignoriert) zwischengespeichert wird. Benötigt wird also 
ein Datentyp, der mit Fliesskommazahlen (Floating Point Numbers) klarkommt. Wie 
würden sie eine solche Fliesskommazahl definieren, und wie sie digital abspeichern? 
Machen sie dazu einen Vorschlag.

**Lösungsweg:**

Um eine Fliesskommazahl (Floating Point Number) zu definieren und digital abzuspeichern, könnte man den Datentyp `float` in vielen Programmiersprachen verwenden. Hier ist ein allgemeiner Vorschlag für die Definition und Speicherung einer Fliesskommazahl:

**Definition:**
In den meisten Programmiersprachen wird der Datentyp `float` für Fliesskommazahlen verwendet. Zum Beispiel in C, C++, Java und vielen anderen Sprachen.

Beispiel in C:
```c
float myFloat = 3.14159;
```

**Digitale Speicherung:**
Fliesskommazahlen werden in der Regel im IEEE 754-Standard für Binärkommazahlen gespeichert. Dieser Standard definiert das Format für die Darstellung von Fliesskommazahlen im Binärformat.

Im IEEE 754-Standard besteht eine 32-Bit-Fliesskommazahl (Single Precision) aus drei Teilen:

1. **Vorzeichenbit (Sign Bit):** 1 Bit, das das Vorzeichen der Zahl darstellt (0 für positiv, 1 für negativ).
2. **Exponent (Exponent):** 8 Bits, die den Exponenten repräsentieren.
3. **Mantisse (Fraction):** 23 Bits, die die Mantisse oder den Bruchteil der Zahl darstellen.

Zum Beispiel könnte die Fliesskommazahl 3.14159 im IEEE 754-Format so aussehen:

```
01000000010010010000111111011011
```

Hier steht das erste Bit für das Vorzeichen (0 für positiv), die nächsten 8 Bits repräsentieren den Exponenten, und die letzten 23 Bits sind die Mantisse.

Es ist wichtig zu beachten, dass Fliesskommazahlen begrenzte Präzision haben, was zu Rundungsfehlern führen kann. Daher sollte man bei Berechnungen mit Fliesskommazahlen Vorsicht walten lassen und sich bewusst sein, dass nicht alle Zahlen exakt dargestellt werden können.

# Auftrag 13
Erstellen sie die Wahrheitstabellen für die folgenden Funktionen:

a. Logisch UND/AND (mit zwei Eingangs- und einer Ausgangsvariablen)

b. Logisch ODER/OR (mit zwei Eingangs- und einer Ausgangsvariablen)

c. Logisch NICHT/NOT (mit einer Eingangs- und einer Ausgangsvariablen) 

d. Logisch EXOR (mit zwei Eingangs- und einer Ausgangsvariablen) 

**Lösungsweg:**

a. Logisch UND/AND (mit zwei Eingangs- und einer Ausgangsvariablen):

**Wahrheitstabelle:**
```
| A | B | A AND B |
|---|---|---------|
| 0 | 0 |    0    |
| 0 | 1 |    0    |
| 1 | 0 |    0    |
| 1 | 1 |    1    |
```

**Schaltplan:**
```plaintext
   +-----+
A -|     |
   | AND |---- A AND B
B -|     |
   +-----+
```

b. Logisch ODER/OR (mit zwei Eingangs- und einer Ausgangsvariablen):

**Wahrheitstabelle:**
```
| A | B | A OR B |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   1    |
| 1 | 0 |   1    |
| 1 | 1 |   1    |
```

**Schaltplan:**
```plaintext
   +-----+
A -|     |
   |  OR |---- A OR B
B -|     |
   +-----+
```

c. Logisch NICHT/NOT (mit einer Eingangs- und einer Ausgangsvariablen):

**Wahrheitstabelle:**
```
| A | NOT A |
|---|-------|
| 0 |   1   |
| 1 |   0   |
```

**Schaltplan:**
```plaintext
   +-----+
A -|     |
   | NOT |---- NOT A
   +-----+
```

d. Logisch EXOR (mit zwei Eingangs- und einer Ausgangsvariablen):

**Wahrheitstabelle:**
```
| A | B | A EXOR B |
|---|---|----------|
| 0 | 0 |    0     |
| 0 | 1 |    1     |
| 1 | 0 |    1     |
| 1 | 1 |    0     |
```

**Schaltplan:**
```plaintext
   +------+
A -|      |
   | EXOR |---- A EXOR B
B -|      |
   +------+
```

Die Schaltpläne verwenden die logischen Gatter (AND, OR, NOT, EXOR) als Basiselemente, und die Verbindungen zwischen den Gattern repräsentieren die logischen Verknüpfungen entsprechend der Wahrheitstabelle.

# Auftrag 14
Eine in der Computertechnik wichtige mathematische Funktion ist die Restwert- oder 
Modulo-Funktion mit dem in z.B. Java und C verwendeten Operationszeichen %. 
Versuchen sie nun die folgende Berechnungen auszuführen. Was stellen sie fest?

a. 11 % 2 = ?<br>
b. 10 % 2 = ?<br>
c. 10 % 3 = ?<br>
d. 10 % 5 = ?<br>
e. 10 % 9 = ?<br>

**Lösungsweg:**

Die Modulo-Funktion gibt den Rest der Division zweier Zahlen an. Hier sind die Berechnungen für die gegebenen Beispiele:

a. \( 11 \% 2 = 1 \)

b. \( 10 \% 2 = 0 \)

c. \( 10 \% 3 = 1 \)

d. \( 10 \% 5 = 0 \)

e. \( 10 \% 9 = 1 \)

Das Ergebnis der Modulo-Operation ist der Rest der Division der beiden Zahlen. Wenn das Ergebnis 0 ist, bedeutet dies, dass die erste Zahl ohne Rest durch die zweite Zahl teilbar ist. Wenn das Ergebnis nicht 0 ist, bleibt der Rest der Division. In diesem Fall bedeutet beispielsweise \(10 \% 2 = 0\), dass 10 durch 2 ohne Rest teilbar ist, während \(11 \% 2 = 1\) bedeutet, dass bei der Division von 11 durch 2 ein Rest von 1 verbleibt.

# Aufgabe zu Notepad++ und HxD
Sie erhalten eine ZIP-Datei switzerland.zip unter folgendem Link: 

https://juergarnold.ch/Codesysteme/switzerland.zip 

Laden sie die ZIP-Datei auf ihren Notebook und extrahieren sie die binäre Datei switzerland.bin. Untersuchen sie diese mit Notepad++ und HxD. In der Datei verstecken sich vier vorzeichenlose 16-Bit-Ganzzahlen. Jede davon hat einen Bezug zur Schweiz. Wandeln sie die vier Zahlen je in ihr Dezimaläquivalent um und geben sie einen Tipp ab, was deren CH-Bedeutung sein kann. 

Die Datein enthält 4 * 16Bit-Zahlen
Eine 16-Bit Zahl entspricht 4Hex-Ziffern

Somit heisst es

050B = 1'291
A145 = 41'285
121A = 4'634
1F9A = 8'090

# Aufgaben zu ASCII und Unicode

Sie erhalten eine ZIP-Datei Textsamples.zip unter folgendem Link:

https://juergarnold.ch/Codesysteme/Textsamples.zip 

Laden sie die ZIP-Datei auf ihren Notebook und extrahieren sie die drei Dateien Textsample1, Textsample2 und Textsample3. Eine der drei Dateien ist in ASCII codiert, die andere in UTF-8 und die dritte in UTF-16. Beantworten sie nun die folgenden Fragen: 

1.	Welche der Dateien ist nun ASCII-codiert, welche UTF-8 und welche UTF-16 BE-BOM?

Textsample1=ASCII, Textsample2=UTF8, Textsample3=UTF16BE

2. Alle drei Dateien enthalten denselben Text aus wie vielen Zeichen besteht dieser?

68 Zeichen

3. Was sind die jeweiligen Dateigrössen? (Beachten sie, dass unter Grösse auf Datenträger jeweils 0 Bytes angegeben wird. Dies darum weil beim Windows Dateisystem NTFS kleine Dateien direkt in die MFT (Master File Table) geschrieben werden) Wie erklären sie sich die Unterschiede?

```
Textsample1=68B 68 x 1 B ASCII

Textsample2=71B
31-30-30-E2-82-AC-2E
31-30-30 = 100
E2 = 1110'0010 somit folgen 2 weitere  Bytes
Damit ergibt sich für das $-Zeichen 3 Byte: E2-A2-AC
66B + 2B + 3B=71
E2-A2-AC=1110'0010-1010'0010-1010'1100

Textsample3=138B
UTF16-BE BOM (Big-Endian) -> Code beginnt mit FE FF =2B
Unicodezeichen werden auf zwei Bytes abgebildet
z.B. Eurozeichen=20AC
Ergibt 2 x 68B + 2B = 138B
```
4.	Bei den weiteren Fragen interessieren uns nur noch die ASCII- und die UTF-8-Datei: Bekanntlich ist UTF-8 in den ersten 128 Zeichen deckungsgleich mit ASCII. Untersuchen sie nun die beiden HEX-Dumps und geben sie an, welche Zeichen unterschiedlich codiert sind. Ein kleiner Tipp: Es sind deren zwei.

Der Buchstabe ä aus dem Wort Parität und das Eurozeichen.

5.	Was bedeuten die beiden Ausdrücke, denen wir z.B. bei UTF-16 begegnen: Big-Endian (BE), Little-Endian (LE)?

BigEndian: hh:mm:ss
LittleEndian: dd:mm:yyyy

# Reflexion

**Unterrichtsinhalte und Ziele:**

In diesem Unterricht war mein Ziel den Stoff, den ich letzte Woche verpasst habe nachzuholen. Ich habe dieses Ziel meiner Meinung nach ziemlich gut erreicht, da ich meine Arbeit heute Morgen fertig geschaft habe.

**Unterrichtsresultate:**

Die Unterrichtsresultate sind hier auf meinem GitHub und auf meinem OneNote ersichtbar, wobei man nur meine Inhalte die ich auf GitHub dokumentiert habe einsehbar sind, da ich nur Notizen in mein OneNote einschreibe.

**Probleme/Knacknüsse:**

Ich fand die Aufgaben 9-13 ziemlich hart, bei diesen Aufgaben hatte ich länger überlegen müssen. Ich habe diese jedoch mit ein wenig recherche selbst lösen können, jedoch will ich diese trotzdem nochmals im nächsten Unterricht anschauen.

**Neue Applikationen, Werkzeuge, Kommandos, etc.:**

--Keine Neue Applikationen, Werkzeuge, Kommandos oder weiteres genutzt--

**Offene Fragen:**
Ich habe folgende Fragen:

- [X] Für was brauch man `LSB` und `MSB`. Wie sollte ich dies interpretieren.

- [X] Wie rechnet man Negative Ganzzahlen in binär um.

- [X] Floats

- [X] Octal zahlen wieso?

- [ ] Aufgabe 9-13 anschauen
