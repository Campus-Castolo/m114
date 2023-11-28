# Auftrag 1.

Welche der Dateien ist nun ASCII-codiert, welche UTF-8 und welche UTF-16 BE-BOM?

- Textsample1: ASCII-codiert (68 Bytes)
- Textsample2: UTF-8 (71 Bytes)
- Textsample3: UTF-16 BE-BOM (138 Bytes)

# Auftrag 2.

Alle drei Dateien enthalten denselben Text. Aus wie vielen Zeichen besteht dieser?

Da jede Zeichenkette "Parität Schweizer-Franken zu Euro bedeutet: 100CHF entsprechen 100€" ist, besteht der Text in allen Dateien aus 78 Zeichen.

# Auftrag 3.

Was sind die jeweiligen Dateigrößen?

- Textsample1 (ASCII): 68 Bytes
- Textsample2 (UTF-8): 71 Bytes
- Textsample3 (UTF-16 BE-BOM): 138 Bytes

Die Unterschiede in der Dateigröße können durch die unterschiedlichen Codierungen und Dateiformate erklärt werden.

# Auftrag 4. 

Bei den weiteren Fragen interessieren uns nur noch die ASCII- und die UTF-8-Datei: Untersuchen sie nun die beiden HEX-Dumps und geben sie an, welche Zeichen unterschiedlich codiert sind. Ein kleiner Tipp: Es sind deren zwei.

Hier wären die entsprechenden HEX-Dumps erforderlich, um die unterschiedlich codierten Zeichen zu identifizieren. Bitte stelle die HEX-Dumps zur Verfügung, damit ich dir dabei helfen kann.

# Auftrag 5. 

Was bedeuten die beiden Ausdrücke, denen wir z.B. bei UTF-16 begegnen: Big-Endian (BE), Little-Endian (LE)?

- Big-Endian (BE): Die Bytes werden in der Reihenfolge von höherwertigem zu niederwertigem Byte gespeichert.
- Little-Endian (LE): Die Bytes werden in der Reihenfolge von niederwertigem zu höherwertigem Byte gespeichert.

# Auftrag 6. 

Im Notepad++ kann man unter dem Menüpunkt Codierung von ASCII zu UTF umschalten. Spielen sie damit etwas herum und notieren sie sich, was in der Darstellung jeweils ändert.

Die Länge des Textes variert, da es immer anderst codiert ist.

# Auftrag 7.

Für Anspruchsvolle: Der UTF-8-Code kann je nach Zeichen ein, zwei, drei oder vier Byte lang sein. Wie kann der Textreader erkennen, wann ein UTF-8 Zeichencode beginnt und wann er endet? Untersuchen sie dies anhand der beiden Textsamples und lesen sie in z.B. Wikipedia die entsprechende Theorie zu UTF-8 durch. Tipp: Startbyte und Folgebyte.

Untersuchen Sie mithilfe eines Hexeditors und eines Texteditors Ihrer Wahl die folgenden Dateien:

1. **Sample1_ascii**: Die ASCII-Datei enthält vier Zeichen aus dem 7-Bit ASCII-Bereich (z.B. BERN).

2. **Sample2_utf8**: Die UTF-8-Datei enthält ebenfalls vier Zeichen aus dem 7-Bit ASCII-Bereich (identisch mit Sample1, da 7-Bit ASCII-Zeichen verwendet werden).

3. **Sample3_ascii**: Die ASCII-Datei enthält vier 8-Bit ANSI-ASCII-Zeichen, darunter ein "ü" gemäß ISO-Standard 8859-2 (z.B. Züri). Dies verwendet den erweiterten 8-Bit ASCII-Zeichensatz.

4. **Sample4_utf8**: Die UTF-8-Datei enthält ebenfalls vier Zeichen, darunter das "ü" mit dem Unicode "U+00FC" (z.B. Züri). Beachten Sie, dass das "ü" in UTF-8 nun 2 Bytes benötigt.

5. **Sample5_utf8**: Die UTF-8-Datei enthält vier chinesische Zeichen (z.B. Berufsschule). Jedes chinesische Zeichen benötigt 24 Bit.

Was fällt Ihnen bezüglich der Länge und Codierung der UTF-8-Zeichen im Vergleich zu den ASCII-Zeichen auf?

Bei den ASCII-Dateien benötigt jedes Zeichen nur wenige Bits. Im Gegensatz dazu variiert die Länge der UTF-8-Codierung zwischen 1 bis 4 Byte.

Erstellen Sie ein Word-File mit Schriftzeichen, die Ihre PC-Tastatur nicht zur Verfügung stellt, wie z.B. das Euro-Zeichen. Nutzen Sie dabei die im Theorieteil vorgestellten UTF-8-Eingabemethoden. Für diese Aufgabe, da sie auf individuellen Eingaben und Erfahrungen basiert.

# Reflexion

**Unterrichtsinhalte und Ziele:**

In diesem Learning Session war mein Ziel den Stoff, den ich durch das Krank sein verpasst habe gut nachzuholen und alles verpasst habe verständlich zu machen.

**Unterrichtsresultate:**

Die Unterrichtsresultate sind hier auf meinem GitHub.

**Probleme/Knacknüsse:**

Ich hatte nicht wirklich grosse Probleme die einzigen Probleme die ich hatte war einfach die Eintteilung den Stoff selber nachzuholen.

**Neue Applikationen, Werkzeuge, Kommandos, etc.:**

--Keine Neue Applikationen, Werkzeuge, Kommandos oder weiteres genutzt--

**Offene Fragen:**
Ich habe folgende Fragen:

- [ ] Wie kommt das mit den Datei Grössen genau zu Stande
