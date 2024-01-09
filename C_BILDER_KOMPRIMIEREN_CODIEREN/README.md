# Auftrag 1
Bestimmen sie die Farben für die folgenden RGB-Farbcodes (in HEX). Nutzen sie den RGB-Farbenmixer:

•	#FF0000 entspricht der Farbe ....<br>
•	#00FF00 entspricht der Farbe ....<br>
•	#0000FF entspricht der Farbe ....<br>
•	#FFFF00 entspricht der Farbe ....<br>
•	#00FFFF entspricht der Farbe ....<br>
•	#FF00FF entspricht der Farbe ....<br>
•	#000000 entspricht der Farbe ....<br>
•	#FFFFFF entspricht der Farbe ....<br>
•	#00BC00 entspricht der Farbe ....<br>

**Lösungsweg:**<br>
Um dies Aufgabe zu lösen ist die Folgende Grafik sehr Hilfreich:

![Alt text](img/image-1.png)

Um diese Aufgabe zu verstehen muss man verstehen, wie eine Farbe Hexadezimal angezeigt wird.

`#FF0000` Diese Hexadezimale Zahl kann man in drei zweier paare unterteilen das erste in diesem Beispiel `FF` steht für den Rotfarben-Kanal. der Hexadezimale Wert `FF` repräsentiert die Dezimalzahl `255`. Das zweite paar repräsentiert den Grünfarben-Kanal. Der Hexadezimale Wert `00` repräsentiert die Dezimalzahl `0`, dies heisst das keine Grüntöne in dieser Farbe vorhanden sind. Das dritte paar `00` repräsentiert den Blaufarben-Kanal. Der Hexadezimale Wert `00` repräsentiert die Dezimalzahl `0`, dies heisst das keine Blautöne in dieser Farbe vorhanden sind.

Das heisst das die erste Farbe `#FF0000` den RGB-Farbcode `255 000 000` hat. Dies heisst diese Farbe ist `ROT`

- `#FF0000` entspricht der Farbe Rot und hat den RGB-Farbcode (255, 0, 0).
- `#00FF00` entspricht der Farbe Grün und hat den RGB-Farbcode (0, 255, 0).
- `#0000FF` entspricht der Farbe Blau und hat den RGB-Farbcode (0, 0, 255).
- `#FFFF00` entspricht der Farbe Gelb und hat den RGB-Farbcode (255, 255, 0).
- `#00FFFF` entspricht der Farbe Cyan und hat den RGB-Farbcode (0, 255, 255).
- `#FF00FF` entspricht der Farbe Magenta und hat den RGB-Farbcode (255, 0, 255).
- `#000000` entspricht der Farbe Schwarz und hat den RGB-Farbcode (0, 0, 0).
- `#FFFFFF` entspricht der Farbe Weiß und hat den RGB-Farbcode (255, 255, 255).
- `#00BC00` entspricht der Farbe Grün (Nuance) und hat den RGB-Farbcode (0, 188, 0).

# Auftrag 2
Bestimmen sie die Farben für die folgenden prozentualen CMYK-Angaben. Nutzen sie den CMYK-Farbenmixer:

•	C:0%, M:100%, Y:100%, K:0% entspricht der Farbe ....<br>
•	C:100%, M:0%, Y:100%, K:0% entspricht der Farbe ....<br>
•	C:100%, M:100%, Y:0%, K:0% entspricht der Farbe ....<br>
•	C:0%, M:0%, Y:100%, K:0% entspricht der Farbe ....<br>
•	C:100%, M:0%, Y:0%, K:0% entspricht der Farbe ....<br>
•	C:0%, M:100%, Y:0%, K:0% entspricht der Farbe ....<br>
•	C:100%, M:100%, Y:100%, K:0% entspricht der Farbe ....<br>
•	C:0%, M:0%, Y:0%, K:100% entspricht der Farbe ....<br>
•	C:0%, M:0%, Y:0%, K:0% entspricht der Farbe ....<br>
•	C:0%, M:46%, Y:38%, K:22% entspricht der Farbe ....<br>

**Lösungsweg:**<br>
Um dies Aufgabe zu lösen ist die Folgende Grafik sehr Hilfreich:

![Alt text](img/image-2.png)

Die prozentualen CMYK-Angaben beschreiben den Farbaufbau wie folgt:

- **Cyan (C):** 0% - Es wird keine Cyan-Farbe verwendet.
- **Magenta (M):** 100% - Die Farbe besteht vollständig aus Magenta.
- **Yellow (Y):** 100% - Die Farbe besteht vollständig aus Yellow.
- **Key/Black (K):** 0% - Es wird kein Schwarz verwendet.

Daher ergibt sich aus diesen Angaben die Farbe:

- **Farbe:** Ein intensives Gelb.

Zusammengefasst lautet die Lösung:

`C: 0%, M: 100%, Y: 100%, K: 0%` entspricht der Farbe **intensives Gelb**.

- `C:0%, M:100%, Y:100%, K:0%` entspricht der Farbe **Gelb**.
- `C:100%, M:0%, Y:100%, K:0%` entspricht der Farbe **Magenta**.
- `C:100%, M:100%, Y:0%, K:0%` entspricht der Farbe **Cyan**.
- `C:0%, M:0%, Y:100%, K:0%` entspricht der Farbe **Gelb**.
- `C:100%, M:0%, Y:0%, K:0%` entspricht der Farbe **Rot**.
- `C:0%, M:100%, Y:0%, K:0%` entspricht der Farbe **Grün**.
- `C:100%, M:100%, Y:100%, K:0%` entspricht der Farbe **Weiß**.
- `C:0%, M:0%, Y:0%, K:100%` entspricht der Farbe **Schwarz**.
- `C:0%, M:0%, Y:0%, K:0%` entspricht der Farbe **Weiß**.
- `C:0%, M:46%, Y:38%, K:22%` entspricht einer spezifischen Farbmischung.

# Auftrag 3
Berechnen sie den Speicherbedarf für ein unkomprimiertes Einzelbild im HD720p50-Format bei einer True-Color-Farbauflösung.


**Lösungsweg:**<br>
Um den Speicherbedarf für ein unkomprimiertes Einzelbild im HD720p50-Format zu berechnen, benötigen wir einige Informationen. HD720p50 hat eine Auflösung von 1280x720 Pixeln und eine Bildwiederholrate von 50 Bildern pro Sekunde. True-Color bedeutet in der Regel 24 Bit pro Pixel (8 Bit pro Farbkanal).

Die Formel für den Speicherbedarf (in Bytes) pro Bild lautet:

```markdown
Speicherbedarf = (Breite in Pixel) × (Höhe in Pixel) × (Bit pro Pixel) / 8
```

Hier sind die Werte für HD720p50:

- Breite: 1280 Pixel
- Höhe: 720 Pixel
- Bit pro Pixel: 24 (True-Color, also 8 Bit pro Farbkanal für Rot, Grün und Blau)

Setzen wir diese Werte in die Formel ein:

```markdown
Speicherbedarf = (1280 × 720 × 24) / Byte
```
Um den Speicherbedarf in Bytes zu erhalten, teilen wir das Ergebnis durch 8 (weil 1 Byte = 8 Bit):

```markdown
Speicherbedarf = (1280 × 720 × 24) / 8 Byte
```

Die resultierende Zahl gibt den Speicherbedarf für ein Einzelbild im HD720p50-Format in Bytes an.


Es sieht so aus, als ob die Formatierung möglicherweise in Markdown für GitHub angepasst werden muss. Hier ist der Code in einer GitHub-freundlichen Markdown-Formatierung:



Jetzt, um die spezifischen Werte für HD720p50 einzusetzen:

```markdown
Speicherbedarf = (1280 × 720 × 24) / 8 Byte
```

Das Ergebnis dieses Ausdrucks gibt den Speicherbedarf für ein Einzelbild im HD720p50-Format in Bytes an. Beachten Sie, dass GitHub-Markdown keine direkten mathematischen Formeln unterstützt, daher ist dies eine einfache textbasierte Darstellung. Wenn Sie eine detailliertere mathematische Darstellung wünschen, sollten Sie andere Tools oder Formate verwenden.

# Auftrag 4
Welchen Speicherbedarf hat das Video aus der vorangegangenen Aufgabe bei einer Spieldauer von 3 Minuten?

**Lösungsweg:**<br>
Um den Speicherbedarf für das gesamte Video zu berechnen, müssen wir den Speicherbedarf pro Bild mit der Anzahl der Bilder multiplizieren, die pro Sekunde im Video erscheinen, und dies dann mit der Gesamtdauer des Videos in Sekunden multiplizieren. Die Formel lautet:

```markdown
Speicherbedarf für das Video = Speicherbedarf pro Bild x Bilder pro Sekunde x Gesamtdauer des Videos in Sekunden
```

Nun, für HD720p50:

- Bilder pro Sekunde (BPS): 50 (da es sich um HD720p50 handelt)
- Gesamtdauer des Videos: 3 Minuten

Hier ist die Formel in Markdown:

```markdown
Speicherbedarf für das Video = (Breite in Pixel × Höhe in Pixel × Bit pro Pixel / 8) × Bilder pro Sekunde × Gesamtdauer des Videos in Sekunden
```

Setzen Sie die spezifischen Werte für HD720p50 ein:

```markdown
Speicherbedarf für das Video = (1280 × 720 × 24 / 8) × 50 × 3 × 60
```

Das Ergebnis dieses Ausdrucks gibt den Gesamtspeicherbedarf für das Video in Bytes an. Um dies in größere Einheiten wie Megabyte oder Gigabyte zu konvertieren, können Sie das Ergebnis durch \( 1024 \times 1024 \) bzw. \( 1024 \times 1024 \times 1024 \) teilen.

# Auftrag 5
Ihre Digitalkamera bietet für die Speicherung ihrer Bilder folgende Formate an: RAW, TIF, JPG. Erklären sie in ein paar kurzen Sätzen die Unterschiede und Einsatzgebiete dieser drei Formatvarianten.

**Lösungsweg:**<br>
Die Formate RAW, TIF und JPG sind verschiedene Dateiformate, die in der Fotografie für die Speicherung von Bildern verwendet werden. Hier sind die Unterschiede und Einsatzgebiete in kurzen Sätzen erklärt:

1. **RAW (Rohdaten):** RAW ist ein unkomprimiertes Dateiformat, das alle Daten enthält, die von der Kamera aufgenommen wurden, ohne Verluste durch Kompression. Es bietet die höchste Qualität und Flexibilität bei der Bildbearbeitung, da es alle Bilddaten im Originalzustand speichert. Fotografen, die intensive Bearbeitungen vornehmen möchten, nutzen oft das RAW-Format. Es hat jedoch den Nachteil größerer Dateigrößen.

2. **TIF (Tagged Image File Format):** TIF ist ein verlustfreies, unkomprimiertes oder komprimiertes Dateiformat, das eine hohe Bildqualität beibehält. Es unterstützt auch Ebenen und ist weit verbreitet in der professionellen Bildbearbeitung und Druckindustrie. TIF-Dateien sind jedoch größer als JPG und eignen sich besonders für die Langzeitarchivierung von Bildern in höchster Qualität.

3. **JPG (Joint Photographic Experts Group):** JPG ist ein komprimiertes Dateiformat, das Verluste in der Bildqualität aufweisen kann, da es Informationen für eine kleinere Dateigröße komprimiert. Es ist ideal für den Alltagsgebrauch, Online-Veröffentlichungen und Situationen, in denen Dateigröße wichtig ist. JPG eignet sich weniger für intensive Bildbearbeitung, da jede erneute Speicherung zu weiterem Qualitätsverlust führen kann.

In Zusammenfassung: RAW bietet höchste Qualität und Bearbeitungsfreiheit, TIF bietet Verlustfreiheit und wird oft für professionelle Zwecke verwendet, während JPG für den alltäglichen Gebrauch und die effiziente Speicherung von Bildern geeignet ist, jedoch mit einem gewissen Qualitätsverlust.
