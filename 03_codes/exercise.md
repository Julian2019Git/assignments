# 3. Codes - Übungen

<!-- Chapter: 3 -->

## 3.1 Morse-Alphabet
Warum werden beim Morse-Alphabet manche Buchstaben mit kurzen und manche mit langen Folgen der Zeichen `.` und `-` dargestellt? Handelt es sich beim Morse-Alphabet um eine binäre Codierung? Begründen Sie Ihre Antwort.


## 3.2 Fano-Bedingung
Genügt die Deutsche Sprache der Fano-Bedingung? Begründen Sie Ihre Antwort.


## 3.3 Hamming-Distanz bestimmen
Bestimmen Sie die Hamming-Distanz für den folgenden Code: { 110101, 101011, 010011, 101100 }

  * [ ] 1
  * [ ] 2
  * [ ] 3
  * [ ] 4
  * [ ] 5
  * [ ] 6

## 3.4 Hamming-Distanz bestimmen
Bestimmen Sie die Hamming-Distanz für den folgenden Code: { 2B, 4A, 78, A9 }

  * [ ] 1
  * [ ] 2
  * [ ] 3
  * [ ] 4
  * [ ] 5
  * [ ] 6

## 3.5 Hamming-Distanz anpassen
Bestimmen Sie die Hamming-Distanz für den Code {1101011, 1010110, 0000011, 0001100} und modifizieren Sie diesen Code dann durch Änderung eines einzigen Bit so, dass sich eine um eins erhöhte Hamming-Distanz ergibt.

Welcher Code ergibt sich dann?


## 3.6 Parität
Geben Sie für die folgenden Bitfolgen jeweils das Paritätsbit an.

  * `0000000`
  * `0000010`
  * `1000000`
  * `1001001`
  * `1111111`
  * `1010101`


## 3.7 Parität
Geben Sie für die Bitfolgen `1000111001` das Paritätsbit bei _gerader (even)_ Parität an.


## 3.8 Parität
Geben Sie für die Bitfolgen `1001100001` das Paritätsbit bei _gerader (even)_ Parität an.


## 3.9 Serielle Daten dekodieren
Bei einer seriellen Datenübermittlung werden mit 7 Bit codierte ASCII-Zeichen mit einem zusätzlichen Paritätsbit und einem Längsprüfwort nach jeweils 8 Zeichen gesendet. Es gilt gerade Parität. Es wird folgende Nachricht empfangen:

```console
1000110 1
0110010 0
1100101 0
1101001 0
1100010 1
1101001 0
1100101 0
1110010 0

0100100 0
```

Wie lautet die empfangene Nachricht? Sind Übertragungsfehler aufgetreten? Wenn ja, wie lautet die korrekte Nachricht?


## 3.10 CRC-Prüfsumme berechnen
Berechnen Sie für die Nachricht `1101011010` die CRC-Prüfsumme mit dem Prüfpolynom `10011`.


  * [ ] 11010110101000
  * [ ] 11010110101101
  * [ ] 11010110101001
  * [ ] 11010110101111
  * [ ] 10010100101111

## 3.11 Daten mit CRC prüfen
Sie haben die Nachricht `100110110101` erhalten. Das Prüfpolynom ist `10011`. Ist die Nachricht korrekt übertragen worden?

  * [ ] Ja
  * [ ] Nein

## 3.12 Komprimierung mit RLE
Komprimieren Sie das folgende Bild mit Hilfe eines Run-Length-Encodings (RLE). Geben Sie das Ergebnis an. Verwenden Sie der Einfachheit halber für alle Pixel eine Längenangabe und verzichten Sie auf das Markierungsbyte. Sie können anstatt der Byte-Folge einen Buchstaben für jede Farbe verwenden, z.B. `w` für weiß, `b` für blau etc.

![](img/ghost.png)

Wieviel Platz spart Ihre Codierung im Vergleich zu einer Speicherung ohne Kompression?


## 3.13 Huffman-Code bestimmen
Erstellen Sie für das folgende Bild einen Huffman Code und codieren Sie es damit

![](img/bird.png)


## 3.14 Huffman-Code bestimmen
Gegeben ist folgende Häufigkeitsverteilung für eine Menge von Zeichen:

| Zeichen       | R | I | C | H | T | G |
|---------------|---|---|---|---|---|---|
| Häufigkeit [%]|25 |21 |19 |18 |13 |4  |

Generieren Sie einen Huffman-Code für die angegebene Menge

Dekodieren Sie folgende Nachricht (von links nach rechts!) `0010110100110100111` mittels des generierten Code.


## 3.15 Verlustfreie- und Verlustbehaftete Kompression
Geben Sie für die folgenden Verfahre an, ob sie verlustbehaftete oder verlustfreie Kompressionsverfahren sind:

  * RLE
  * LZ77
  * LZW
  * MP3
  * H.264 (MPEG-4)
  * FLAC
  * GZIP
  * JPEG


## 3.16 Verlustfreie- und Verlustbehaftete Kompression
Geben Sie für die folgenden Verfahre an, ob sie verlustbehaftete oder verlustfreie Kompressionsverfahren sind:

  * LZW: ....
  * MP3: ....
  * H.264 (MPEG-4): ....
  * JPEG: ....
  * GZIP: ....
  * LZ77: ....
  * FLAC: ....
  * RLE: ....

*Antworten:*

  1. verlustfrei
  2. verlustbehaftet


## 3.17 Vektorgrafik vs. Bitmap
  1. Wie funktioniert die Speicherung von Bildern als _Vektorgrafiken_? Welche Datei-Formate kennen Sie?
  2. Wie funktioniert die Speicherung von Bildern als _Bitmaps_ bzw. _Rastergrafiken_? Welche Datei-Formate kennen Sie?
  3. Welches Format sollte man für welche Art von Bildern/Grafiken einsetzen?


## 3.18 Speicherverbrauch eines Bildes
Das folgende Bild (Auflösung 640x466 Pixel) hat mit JPEG-Kompression (75% Qualität) eine Größe von 111.431 Byte.

<img src="img/jpeg-testbild.jpg" width="300">

  1. Wie viel Speicher würde man benötigen, wenn man es unkomprimiert ablegen wollte. Gehen Sie von 8 Bit pro Farbe ohne Alphakanal aus. Ignorieren Sie die Header und Metadaten.
  2. Wie stark ist somit die Kompression, d.h. um welchen Faktor wird das Bild durch sie kleiner?


## 3.19 GIF oder JPEG für Comics
Warum ist das GIF-Dateiformat besser geeignet, um farbige Comics zu speichern, als JPEG? Gibt es noch ein anderes Bildformat, dass sich für Comics eignet und das möglicherweise noch besser als GIF ist?


## 3.20 Grafikformate
Es gibt unterschiedliche Grafikformate mit ebenso unterschiedlichen Eigenschaften. Ordnen Sie bitte die Eigenschaften den Formaten zu:

  * BMP: ....
  * JPEG: ....
  * GIF: ....
  * TIFF: ....
  * PNG: ....
  * SVG: ....

*Antworten:*

  1. pixelbasiert, verlustfrei, echtfarben, komprimiert
  2. pixelbasiert, verlustfrei oder verlustbehaftet, echtfarben, komprimiert
  3. vektorbasiert, verlustbehaftet
  4. pixelbasiert, verlustfrei, maximal 256 Farben, komprimiert
  5. vektorbasiert, verlustfrei
  6. pixelbasiert, verlustfrei, echtfarben, unkomprimiert
  7. pixelbasiert, verlustbehaftet, echtfarben, komprimiert
  8. pixelbasiert, verlustbehaftet, maximal 256 Farben, komprimiert


## 3.21 JPEG in der Fotografie
Viele Fotografen speichern ihre Bilder, solange sie diese noch bearbeiten, im TIFF-Format und erzeugen JPEGs erst ganz am Ende der Bearbeitung. Warum?


## 3.22 Funktionsweise von MP3
Welche Eigenschaft des menschlichen Hörsinns wird vom MP3-Format genutzt?


## 3.23 Funktionsweise von MP3
Welche Eigenschaft der folgenden Eigenschaften trifft auf das MP3-Format zu?

  * [ ] bedient sich der Psychologie
  * [ ] basiert auf dem Shannon-Theorem
  * [ ] bedient sich der Psychoakustik
  * [ ] speichert nur für den Menschen wahrnehmbare Anteile des Signals
  * [ ] bedient sich der Trägheit der Luft als Medium
  * [ ] ist verlustfrei
  * [ ] reduziert die Auflösung des Signals in allen Frequenzbereichen
  * [ ] verringert die Datenmenge im Vergleich zu WAV
  * [ ] hat eine konstante Bitrate
  * [ ] ist verlustbehaftet
  * [ ] hat eine variable Bitrate

## 3.24 Speicherverbrauch eines Bildes
Ein Bild (Auflösung 640x466 Pixel) hat mit JPEG-Kompression (75% Qualität) eine Größe von 111.431 Byte. Wie viel Speicher würde man benötigen, wenn man es unkomprimiert ablegen wollte. Gehen Sie von 8 Bit pro Farbe ohne Alphakanal aus. Ignorieren Sie die Header und Metadaten.



  1. Wie stark ist somit die Kompression, d.h. um welchen Faktor wird das Bild durch sie kleiner?

  * [ ] 298.240 Byte
  * [ ] 894.720 Byte
  * [ ] 2.385.920 Byte
  * [ ] 7.157.760 Byte

## 3.25 Kompressionsfaktor JPEG
Ein Bild (Auflösung 640x466 Pixel) hat mit JPEG-Kompression (75% Qualität) eine Größe von 111.431 Byte. Berechnen Sie, wie viel Speicher man benötigen würde, um es unkomprimiert abzulegen. Gehen Sie von 8 Bit pro Farbe ohne Alphakanal aus. Ignorieren Sie die Header und Metadaten. Berechnen Sie dann die wie stark die Kompression ist, d.h. um welchen Faktor das Bild durch sie kleiner wurde.

  * [ ] ca. 4
  * [ ] ca. 6
  * [ ] ca. 8
  * [ ] ca. 10
  * [ ] ca. 12
  * [ ] ca. 14
  * [ ] ca. 20
  * [ ] ca. 40

## 3.26 Huffman-Code bestimmen
Gegeben ist folgende Häufigkeitsverteilung für eine Menge von Zeichen:

| Zeichen       | R | I | C | H | T | G |
|---------------|---|---|---|---|---|---|
| Häufigkeit [%]|25 |21 |19 |18 |13 |4  |

Generieren Sie einen Huffman-Code für die angegebene Menge

Dekodieren Sie folgende Nachricht (von links nach rechts!) `0010110100110100111` mittels des generierten Code.


