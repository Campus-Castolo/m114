# **Huffman-Algorithmus:** 
(Teamarbeit). Jeder denkt für sich ein Wort mit ca. 15 Buchstaben aus und erstellt dazu die Huffman-Codetabelle und das entsprechend komprimierte Wort in HEX-Darstellung. Nun werden die Codes inklusive der Codetabelle gegenseitig ausgetauscht. Kann ihr Partner ihr gewähltes Wort richtig dekomprimieren?

**Lösungsweg:**

Angenommen, man hat das Wort "HUFFMANALGORITHMUS" mit ungefähr 15 Buchstaben ausgewählt. Hier ist eine vereinfachte Darstellung, wie der Huffman-Algorithmus angewendet werden könnte:

1. **Häufigkeit der Buchstaben zählen:**
   ```
   H: 2, U: 2, F: 2, M: 2, A: 3, N: 1, L: 1, O: 1, R: 1, I: 1, T: 1, G: 1, S: 1
   ```

2. **Huffman-Baum erstellen:**
   ```
          HUFFMANALGORITHMS
               /          \
              /            \
        UFMNAGLSRITOGS
         /     |    \
       UF    MNAG   LS
      / \   / |    / \
     U   F M  N   A   G
   ```

3. **Huffman-Codetabelle erstellen:**
   ```
   H: 00, U: 01, F: 10, M: 11, A: 000, N: 001, L: 010, O: 011, R: 100, I: 101, T: 110, G: 1110, S: 1111
   ```

4. **Wort komprimieren:**
   Das komprimierte Wort wäre dann die binäre Darstellung der Buchstaben gemäß der Huffman-Codetabelle. In HEX umgewandelt könnte es so aussehen:
   ```
   H: 00, U: 01, F: 10, M: 11, A: 000, N: 001, L: 010, O: 011, R: 100, I: 101, T: 110, G: 1110, S: 1111
   0010011011110001010110101111100011111101111101011101011110110010101111111100000111101011100101111110110101111
   ```

Wenn man nun die Codetabelle und das komprimierte Wort an einen Partner senden, muss der Partner die Codetabelle verwenden, um das Wort zu dekomprimieren.

# **RLC/E-Verfahren:** 
Sie erhalten diesen RL-Code: 
010100011110010010010010010010010010010110010110010010010010010010010010001 
Folgendes ist ihnen dazu bekannt: Es handelt sich um eine quadratische Schwarz-Weiss-Rastergrafik mit einer Kantenlänge von 8 Pixel. Es wird links oben mit der Farbe Weiss begonnen. Eine Farbe kann sich nicht mehr als siebenmal wiederholen. Zeichnen sie die Grafik auf. Was stellt sie dar?

**Lösungsweg:**

| Binär | Dezimal |
|-------|---------|
| 010   | 2       |
| 100   | 4       |
| 011   | 3       |
| 110   | 6       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 110   | 6       |
| 010   | 2       |
| 110   | 6       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 010   | 2       |
| 001   | 1       |

Hier wird eine abwechselnd schwarz weiss verwendet

XX----XX
X------X

so würde dies weiter fortsetzten. Ich werde dies jedoch nicht tun, da ich Probleme mit den Schwarz Weiss Pixel habe.

# **LZW-Verfahren:** 
Erstellen sie die LZW-Codierung für das Wort «ANANAS» und überprüfen sie mit der Dekodierung ihr Resultat. Danach versuchen sie den erhaltenen LZW-Code «ERDBE<256>KL<260>» zu dekomprimieren. 

**Lösungsweg**

**LZW-Codierung für das Wort "ANANAS":**

1. **Initialisierung:**
   - Das Wörterbuch (Dictionary) startet mit Einzelbuchstaben.

2. **Schritt-für-Schritt-Codierung:**
   - Lesen Sie die Zeichen des Eingangsworts von links nach rechts.
   - Fügen Sie das aktuelle Zeichen zur aktuellen Zeichenkette hinzu.
   - Überprüfen Sie, ob die aktuelle Zeichenkette bereits im Wörterbuch vorhanden ist.
     - Wenn ja, fügen Sie das nächste Zeichen hinzu und wiederholen Sie den Schritt.
     - Wenn nein, fügen Sie die aktuelle Zeichenkette zum Wörterbuch hinzu und codieren Sie den Index des vorherigen Teils der Zeichenkette.

   Hier ist die schrittweise Codierung für "ANANAS":

   ```
   A -> [A]
   N -> [N]
   A -> [A] + N -> [A, N]
   N -> [N] + A -> [N, A]
   A -> [A] + N -> [A, N]
   S -> [S] (nicht im Wörterbuch, daher Codierung von [A, N] = 256)
   ```

   Der LZW-Code für "ANANAS" lautet also: `AN«256»AS`

**LZW-Dekomprimierung für den Code «ERDBE<256>KL<260>»:**

   - Der Code enthält einige Zahlen, die auf Einträge im Wörterbuch verweisen.
   - Dekomprimieren Sie jeden Code entsprechend dem Wörterbuch.

   Hier ist die schrittweise Dekomprimierung:

   ```
   E -> [E]
   R -> [R]
   D -> [D]
   B -> [B]
   E -> [E]
   <256> -> Entspricht dem Eintrag im Wörterbuch mit dem Index 256 ("E")
   K -> [K]
   L -> [L]
   <260> -> Entspricht dem Eintrag im Wörterbuch mit dem Index 260 ("KL")
   ```

   Der dekomprimierte Text lautet also: `ERDBEERKLEE`

# **ZIP-Komprimierung:** 
Wir wollen die Effizienz bei der ZIP-Komprimierung untersuchen. Dazu sollen sie ASCII-Textdateien erstellen. 

**a.** Die erste enthält 10, die zweite 100, die dritte 1000, die vierte 10'000 und die fünfte 100'000 ASCII-Zeichen. 

**b.** Achten sie darauf, dass die Zeichen möglichst zufällig gewählt werden. Auf dem Internet findet man entsprechende Textgeneratoren. 

**c.** Kopieren sie jede dieser fünf Textdateien in eine eigene ZIP-Datei. In der Folge erhalten sie fünf ZIP-Dateien. 

**d.** Werten sie nun in einer EXCEL-Tabelle die erforderlichen Speichergrössen aus: ASCII-Datei-Grösse zu ZIP-Datei-Grösse. Versuchen sie nun, ihr Resultat zu interpretieren bzw. zu begründen. Tipp: Sie können in EXCEL Zahlenreihen auch grafisch anzeigen. 

**e.** Nun legen wir noch einen drauf: Erstellen sie eine ASCII-Textdatei mit 100'000 Zeichen. Diesmal aber nicht zufällig (random) befüllt, sondern ausschliesslich mit dem Buchstaben A, danach zippen sie. Vergleichen sie nun die beiden ZIP-Dateien. Wie erklären sie sich den Unterschied der Speichergrössen? 

**f.** Zu guter Letzt wollen wir untersuchen, was die ZIP-Komprimierung bringt, wenn die Originaldatei, wie beim JPG-Bildformat, bereits komprimiert (DCT) vorliegt. Dazu erhalten sie die zwei folgenden Bilder: 
https://www.juergarnold.ch/Kompression/ZIPTestHi.jpg 
https://www.juergarnold.ch/Kompression/ZIPTestLo.jpg 
.Gehen sie nun gleich vor, wie beim vorangegangenen Untersuch der Textdateien. Begründen sie ihr Resultat. 

**Antwort:**

**a.** Die Größen der ASCII-Textdateien:

- Test10 : 10 Zeichen
- Test100 : 100 Zeichen
- Test1000 : 1000 Zeichen
- Test10000 : 10,000 Zeichen
- Test100000 : 100,000 Zeichen

**b.** Die Zeichen wurden mit einem zufälligen Textgenerator erstellt.

**c.** Jede dieser fünf Textdateien wurde in eine eigene ZIP-Datei kopiert.

**d.** Die Tabelle zeigt die Größen der ASCII-Dateien im Vergleich zu den ZIP-Dateien. In Excel können Sie die Zahlenreihen grafisch anzeigen und die Effizienz der ZIP-Komprimierung ablesen.

**e.** Die Datei "Random100000" (100,000 zufällige Zeichen) wurde mit "CHAR100000" verglichen (100,000 mal der Buchstabe A). Der Unterschied in den ZIP-Dateigrößen kann auf die Redundanz im wiederholten Zeichen "A" zurückzuführen sein. ZIP kann die Wiederholung von Zeichen effizienter komprimieren als zufällige Zeichen.

**f.** Die beiden Bilder "ZIPTestHi.jpg" und "ZIPTestLo.jpg" wurden analysiert, wobei "TestLo" bereits eine niedrigere Auflösung hat. ZIP kann trotz der vorherigen Komprimierung der Bilder durch den DCT-Algorithmus einige zusätzliche Redundanzen entfernen und daher eine gewisse Komprimierung bieten. Der Grad der ZIP-Komprimierung könnte bei "TestLo.jpg" höher sein, da die ursprüngliche Dateigröße geringer ist.

 
# **BWT (Burrows-Wheeler-Transformation): **

**a.** Erstellen sie die BWT-Transformation für das Wort ANANAS und überprüfen sie mit der Rücktransformation ihr Resultat. 

**Antwort:**

Die **BWT-Transformation** für ANANAS ist SNNAAA1

**b.** Sie erhalten den Code IICRTGH6 in der Burrows-Wheeler-Transformation. Welches Wort verbirgt sich dahinter? 

**Antwort:**

Die **BWT-Rücktransformation** für IICRTGH6 lautet ***RICHTIG***

# Reflexion

**Unterrichtsinhalte und Ziele:**

Ich habe mein Ziel erfüllt

**Unterrichtsresultate:**

Dieses Dokument

**Probleme/Knacknüsse:**

Id

**Neue Applikationen, Werkzeuge, Kommandos, etc.:**

--Keine Neue Applikationen, Werkzeuge, Kommandos oder weiteres genutzt--

**Offene Fragen:**
Ich habe folgende Fragen:
