# 5. Digitale Logik - Übungen

<!-- Chapter: 5 -->

Hinweis: Die Aufgaben verwenden der Einfachheit halber die Symbole aus Java für die Darstellung der

  * _Konjunktion_ (AND): `&`,
  * _Disjunktion_ (OR): `|` und
  * _Negation_ (NOT): `!`
  * _Exklusiv Oder_ (XOR): `^`

## 5.1 Beweis De Morgansche Gesetz
Beweisen Sie mit Hilfe einer Wahrheitstabelle das De Morgansche Gesetz:
`!(P | Q) = !P & !Q`


## 5.2 Ausdruck in Wahrheitstabelle darstellen
Stellen Sie eine Wahrheitstabelle für folgenden Ausdruck auf (P und Q sind Aussagen, die Wahr `T` oder Falsch `F` sein können): `(P & Q) | (!P & !Q)`


## 5.3 Ausdruck umformen
Vereinfachen Sie durch elementare Umformungen den folgenden Ausdruck: `(A | B) & (!A & B)`. Überprüfen Sie mit einer Wahrheitstabelle, ob das Ergebnis korrekt ist.


## 5.4 Darstellung von Verknüpfungen durch andere
Stellen Sie die zweistelligen logischen Verknüpfungen Implikation, NOR, NAND, Äquivalenz und XOR unter ausschließlicher Verwendung von Konjunktion (AND, `&`), Disjunktion (OR, `|`) und Negation (NOT, `!`) dar.


## 5.5 Disjunktive Normalform
Eine Schaltfunktion y mit drei Eingängen x1, x2, x3 sei durch folgende Funktionstabelle gegeben:

| x1  | x2  | x3  | y  |
|-----|-----|-----|----|
|  0  |   0 |   0 |  0 |
|  0  |   0 |   1 |  1 |
|  0  |   1 |   0 |  1 |
|  0  |   1 |   1 |  0 |
|  1  |   0 |   0 |  0 |
|  1  |   0 |   1 |  1 |
|  1  |   1 |   0 |  1 |
|  1  |   1 |   1 |  1 |

Geben Sie die Schaltfunktion in disjunktiver Normalform an, erstellen Sie das zugehörige KV-Diagramm und vereinfachen Sie die Funktion so weit wie möglich.


## 5.6 Gatter erstellen
Erstellen Sie eine Wertetabelle und einen Schaltplan mit möglichst wenig Gattern für die folgende Schaltfunktion:
`f(x1, x2, x3) = (x1 & x2 & !x3) | (x1 & !x2 & !x3)`.


## 5.7 Logische Funktionen auf Bitfolgen anwenden
Berechnen Sie `(10010100 & !0101111)`:

<div style="border: 1px solid grey;"><br><br><br><br><br><br><br><br><br><br><br><br></div>


## 5.8 Logische Funktionen auf Bitfolgen anwenden
Bitte berechnen Sie `01001011 & 10101011` durch bitweise Anwendung des Operators `&`.

## 5.9 Logische Funktionen auf Bitfolgen anwenden
Bitte berechnen Sie `100000011 & 011101100` durch bitweise Anwendung des Operators `&`.

## 5.10 Logische Funktionen auf Bitfolgen anwenden
Bitte berechnen Sie `11111111 & 00101101` durch bitweise Anwendung des Operators `&`.

## 5.11 Logische Funktionen auf Bitfolgen anwenden
Bitte berechnen Sie `01001011 | 10101011` durch bitweise Anwendung des Operators `|`.

## 5.12 Logische Funktionen auf Bitfolgen anwenden
Bitte berechnen Sie `10000011 | 11101100` durch bitweise Anwendung des Operators `|`.

## 5.13 Logische Funktionen auf Bitfolgen anwenden
Bitte berechnen Sie `11111111 | 00101101` durch bitweise Anwendung des Operators `|`.

## 5.14 Logische Funktionen auf Bitfolgen anwenden
Bitte berechnen Sie `01001011 ^ 10101011` durch bitweise Anwendung des Operators `^`.

## 5.15 Logische Funktionen auf Bitfolgen anwenden
Bitte berechnen Sie `100000011 ^ 011101100` durch bitweise Anwendung des Operators `^`.

## 5.16 Logische Funktionen auf Bitfolgen anwenden
Bitte berechnen Sie `11111111 ^ 00101101` durch bitweise Anwendung des Operators `^`.

## 5.17 Bits in einem Byte umdrehen
Angenommen, Sie wollen die mittleren 4 Bits eines Bytes umdrehen, wie gehen Sie am einfachsten vor (Bitmaske und Operation)?


  * [ ] AND mit 00111100
  * [ ] XOR mit 11000011
  * [ ] OR mit 11000011
  * [ ] XOR mit 00111100
  * [ ] AND mit 11000011
  * [ ] OR mit 00111100

## 5.18 Leistung einer Schaltung
Berechnen Sie für den unten angegebenen Stromkreis, welche Leistung (in Watt) verbraucht wird.


<img src="img/stromkreis_einfach.png" width="300">


## 5.19 Länge eines Kabels USA vs. Europa
In den USA (Netzspannung 120 V) können die Kabel bei gleicher Dicke ungefähr nur ein Viertel (25%) der Länge von Kabeln in Europa (Netzspannung 230V) haben. Warum ist dies so?


## 5.20 Schaltkreis berechnen
Berechnen Sie für den unten angegebenen Stromkreis alle fehlenden Größen.

<img src="img/stromkreis_komplex.png" width="400">


## 5.21 Oder-Gatter mit vier Eingängen
Entwerfen Sie unter Verwendung von Gattern mit zwei Eingängen ein Oder-Gatter mit vier Eingängen.


## 5.22 Bits in einem Byte umdrehen
Angenommen, Sie wollen die mittleren 4 Bits eines Bytes umdrehen, wie gehen Sie am einfachsten vor (Bitmaske und Operation)?


  * [ ] OR mit 11000011
  * [ ] OR mit 00111100
  * [ ] AND mit 00111100
  * [ ] AND mit 11000011
  * [ ] XOR mit 11000011
  * [ ] XOR mit 00111100

## 5.23 DeMorgan

Bei welchen der unten aufgeführten Aussagen handelt es sich um ein DeMorgan'sches Gesetz?

  * [ ] !A & !B <=> !(A | B)
  * [ ] A | B <=> !(!A & !B)
  * [ ] A => B <=> !A | B
  * [ ] A & (B | C) <=> (A & B) | (A & C)
  * [ ] !(A & B) <=> !A | !B
  * [ ] !A | B <=> B | !A

## 5.24 Schaltung entwerfen
Entwerfen Sie eine Schaltung mit Gattern, die prüft ob einer der Passagiere seinen Gurt geschlossen hat (High-Signal vom Gurtsensor). Ist der Platz leer (Low-Signal vom Sitzplatzsensor) so darf auch der Gurt offen sein. Ist der Platz besetzt und der Gurt offen soll die Schaltung ein High-Signal ausgeben. Verknüpfen Sie dann zwei Sitzplätze zu einem Ergebnis-Signal.

Entwerfen Sie zuerst eine Wahrheitstabelle und geben Sie dann eine Schaltung mit Gattern an.


## 5.25 Ausdruck in Wahrheitstabelle darstellen
Stellen Sie eine Wahrheitstabelle für folgenden Ausdruck auf (P und Q sind Aussagen, die Wahr T oder Falsch F sein können): `(P & !Q) | (!P & !Q)`

<div style="border: 1px solid grey;"><br><br><br><br><br><br><br><br><br><br><br><br></div>


## 5.26 Leistung eines Wasserkochers
Auf einem Wasserkocher steht 230V, 5A. Welche elektrische Leistung nimmt das Gerät auf?

  * [ ] 46 W
  * [ ] 235 W
  * [ ] 264 W
  * [ ] 1150 W
  * [ ] 2305 W
  * [ ] 5750 W

## 5.27 Bits maskieren
Angenommen, sie wollen in beliebigen Bitfolgen (8 Bit) die letzten beiden Bits immer auf Null setzen und das erste Bit immer auf Eins setzen, also z.B. aus `00101011` soll `10101000` werden. Wie können Sie dies mit entsprechenden booleschen Operatoren erreichen?


  * [ ] ODER mit `100000000`, danach XOR mit `11111100`
  * [ ] ODER mit `11111100`, danach UND mit `100000000`
  * [ ] XOR mit `100000000`, danach XOR mit `11111100`
  * [ ] UND mit `100000000`, danach ODER mit `11111100`
  * [ ] NOT, danach XOR mit `11111100`
  * [ ] UND mit `11111100`, danach ODER mit `100000000`
  * [ ] XOR mit `11111100`, danach NOT

## 5.28 Ausdruck umformen
Vereinfachen Sie durch elementare Umformungen den folgenden Ausdruck: `(A | B) & (!A & B)`. Welches Ergebnis erhalten Sie?


  * [ ] `A & !B`
  * [ ] `A | !B`
  * [ ] `!A | B`
  * [ ] `A | B`
  * [ ] `A & B`
  * [ ] `!A | !B`
  * [ ] `!A & !B`
  * [ ] `!A & B`

## 5.29 Bits maskieren
Angenommen, sie wollen in beliebigen Bitfolgen (8 Bit) die letzten beiden Bits immer auf Null setzen und das erste Bit immer auf Eins setzen, also z.B. aus `00101011` soll `10101000` werden. Wie können Sie dies mit entsprechenden booleschen Operatoren erreichen?


  * [ ] XOR mit `100000000`, danach XOR mit `11111100`
  * [ ] NOT, danach XOR mit `11111100`
  * [ ] UND mit `11111100`, danach ODER mit `100000000`
  * [ ] ODER mit `100000000`, danach XOR mit `11111100`
  * [ ] ODER mit `11111100`, danach UND mit `100000000`
  * [ ] XOR mit `11111100`, danach NOT
  * [ ] UND mit `100000000`, danach ODER mit `11111100`

## 5.30 Ausdruck umformen
Vereinfachen Sie durch elementare Umformungen den folgenden Ausdruck: `(A | B) & (!A & B)`. Welches Ergebnis erhalten Sie?


  * [ ] `!A & !B`
  * [ ] `!A & B`
  * [ ] `A | B`
  * [ ] `A | !B`
  * [ ] `!A | !B`
  * [ ] `!A | B`
  * [ ] `A & B`
  * [ ] `A & !B`

