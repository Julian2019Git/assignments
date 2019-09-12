# 7. Formale Sprachen und Automaten - Übungen


## 7.1 Parkscheinautomat
Auf einem Parkplatz kostet das Parken 1,50 Euro. Ein Parkscheinautomat akzeptiert 50 Cent, 1 Euro und 2 Euro-Münzen. Nach Einwurf der korrekten Geldsumme liefert er das Ticket und gegebenenfalls das Restgeld. Er besitzt keine Abbruchtaste.

Entwickeln Sie einen Automaten (DEA), der den Parkscheinautomaten realisiert, alle korrekten Geldbeträge akzeptiert und das richtige Restgeld zurückgibt.


## 7.2 Regulärer Ausdruck für Matrikelnummern
Geben Sie einen regulären Ausdruck an, der die Matrikelnummern der Studierenden, die im Sommersemester 2018 angefangen haben (beginnen mit `181` und darauf folgen immer vier Ziffern) matched.

Erweitern Sie den regulären Ausdruck danach auf das Wintersemester 2017. Beachten Sie, dass die Matrikelnummern im Wintersemester mit `172` *und* `173` beginnen können.

Testen Sie Ihren Ausdruck mit verschiedenen Matrikelnummern.


## 7.3 Ersetzen mit einem regulären Ausdruck
Geben Sie einen regulären Ausdruck an, der alle Vorkommen von "e" in einem Text durch "3" ersetzt. Orientieren Sie sich an der Syntax des Unix-Werkzeugs `sed` bei der Angabe des Ausdrucks (extended regular expressions mit der `-E`-Option). Testen Sie den Ausdruck mit Hilfe von `sed`.


  * [ ] `s/e/3/`
  * [ ] `s\e\3\`
  * [ ] `/e/3/`
  * [ ] `s/e/3/g`
  * [ ] `/e/3/g`

## 7.4 Wörter tauschen
Geben Sie einen regulären Ausdruck an, der zwei durch Bindestrich (`-`) verbundene Wörter vertauscht. Z.B. soll aus "Speicher-Fehler" das Wort "Fehler-Speicher" werden. Orientieren Sie sich an der Syntax des Unix-Werkzeugs `sed` bei der Angabe des Ausdrucks (extended regular expressions mit der `-E`-Option). Testen Sie den Ausdruck mit Hilfe von `sed`.


## 7.5 Greedy Match
Was ist damit gemeint, wenn man bei regulären Ausdrücken von einem sogenannten "greedy match" spricht? Geben Sie ein Beispiel an.


## 7.6 Backus-Naur-Form (BNF)
In C müssen Variablennamen nach der folgenden Regel gebildet werden: "Namen bestehen aus Buchstaben und Ziffern; dabei muss das erste Zeichen ein Buchstabe sein. Der Unterstrich zählt als Buchstabe."

Beschreiben Sie diese Regel mit einem Ausdruck in Backus-Naur-Form.

## 7.7 Erweiterte Backus-Naur-Form (EBNF)
Gegeben sei die folgende Grammatik in EBNF-Form

```console
expression = term  { ("+" | "-") term };
term       = factor  { ("*" | "/") factor };
factor     = constant | variable | "(" expression ")";
variable   = "x" | "y" | "z";
constant   = digit {digit} ;
digit      = "0" | "1" ... "9";
```

Geben Sie mindestens vier beispielhafte Ausdrücke an, die von dieser Grammatik beschrieben werden.


## 7.8 50 Affen
Zur Illustration der zeitlichen Komplexität führen Sie folgende Betrachtung durch: Wie wahrscheinlich ist es, dass 50 Affen an 50 Schreibmaschinen in 50 Jahren irgendwann auch die erste Seite von Shakespeares Drama "Hamlet" getippt haben würden (Groß- und Kleinschreibung wird ignoriert)? Machen Sie hierzu plausible Annahmen bzgl. der Zeichenzahl pro Seite und die Anzahl der Anschläge pro Sekunde.


## 7.9 Komplexität und Verständlichkeit
Wenn die Komplexität eines Algorithmus X größer als die eines Algorithmus Y ist, bedeutet dies, dass X schwerer zu verstehen ist als Y? Erläutern Sie Ihre Antwort.


## 7.10 Komplexität bestimmen
Gegeben seien die folgenden Programmfragmente. Geben Sie die jeweilige Ausführungszeit an. Geben Sie den Aufwand mittels der O-Notation an. Sie dürfen davon ausgehen, dass der fehlende Schleifenrumpf eine konstante Ausführungszeit hat.

Fall 1:
```java
for (int i = 0; i < n; i++) {
    // Rumpf
}
```

Fall 2:
```java
for (int i = 0; i < n; i++) {
    // Rumpf
}

for (int k = 0; k < n; k++) {
    // Rumpf
}
```

Fall 3:
```java
for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
      // Rumpf
    }
}
```

Fall 4:
```java
for (int i = 0; i < n; i++) {
    for (int j = 0; j < i; j++) {
        // Rumpf
    }
}
```

Fall 5:
```java
for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
        for (int k = 0; k < n; k++) {
           // Rumpf  
        }        
    }
}
```


## 7.11 Komplexität berechnen
Betrachten Sie folgende Messdaten, die für die Laufzeit eines Programms bei unterschiedlichen Datenmengen (n) ermittelt wurden:

  1. n^3 + 4n^2 + 2n + 12
  2. 2n(8 + log(n))
  3. (8n + 12) / 6
  4. 1 + 2 + 3 + 4 + ... + n
  5. 7 + log(n^3)
  6. 8n + log(n)

Geben Sie den Aufwand mittels der O-Notation an.


## 7.12 Komplexität berechnen
Betrachten Sie folgende Messdaten, die für die Laufzeit eines Programms bei unterschiedlichen Datenmengen (n) ermittelt wurden und ordnen Sie die entsprechende Komplexität (in O-Notation) zu:

  * 2n(8 + log(n)): ....
  * n^4 + 4n^3 + 2n^2 + 12: ....
  * 7 + log(n^4): ....
  * (8n + 12) / 6: ....
  * 8n + log(n): ....
  * 7 + log(n^3): ....
  * n(7 + log(n)): ....
  * n^3 + 4n^2 + 2n + 12: ....
  * 1 + 2 + 3 + 4 + ... + n: ....

*Antworten:*

  1. O(1)
  2. O(n)
  3. O(n^2)
  4. O(n^3)
  5. O(n^4)
  6. O(n^5)
  7. O(log(n))
  8. O(n log(n))
  9. O(n^2 log(n))


## 7.13 Komplexität bestimmen
Gegeben seien das folgenden Programmfragment. Geben Sie den Aufwand mittels der O-Notation an. Sie dürfen davon ausgehen, dass der fehlende Schleifenrumpf eine konstante Ausführungszeit hat.

```java
for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
      // Rumpf
    }
}

for (int k = 0; k < n; k++) {
    // Rumpf
}
```

  * [ ] O(n)
  * [ ] O(n^2)
  * [ ] O(n^3)
  * [ ] O(n^4)
  * [ ] O(n^5)
  * [ ] O(log(n))
  * [ ] O(n log(n))

## 7.14 Komplexität bestimmen
Gegeben seien das folgenden Programmfragment. Geben Sie den Aufwand mittels der O-Notation an. Sie dürfen davon ausgehen, dass der fehlende Schleifenrumpf eine konstante Ausführungszeit hat.

```java
for (int i = 0; i < n; i++) {
    // Rumpf
}
```

  * [ ] O(n)
  * [ ] O(n^2)
  * [ ] O(n^3)
  * [ ] O(n^4)
  * [ ] O(n^5)
  * [ ] O(log(n))
  * [ ] O(n log(n))

## 7.15 Komplexität bestimmen
Gegeben seien das folgenden Programmfragment. Geben Sie den Aufwand mittels der O-Notation an. Sie dürfen davon ausgehen, dass der fehlende Schleifenrumpf eine konstante Ausführungszeit hat.

```java
for (int i = 0; i < n; i++) {
    // Rumpf
}

for (int k = 0; k < n; k++) {
    // Rumpf
}
```


  * [ ] O(n)
  * [ ] O(n^2)
  * [ ] O(n^3)
  * [ ] O(n^4)
  * [ ] O(n^5)
  * [ ] O(log(n))
  * [ ] O(n log(n))

## 7.16 Komplexität bestimmen
Gegeben seien das folgenden Programmfragment. Geben Sie den Aufwand mittels der O-Notation an. Sie dürfen davon ausgehen, dass der fehlende Schleifenrumpf eine konstante Ausführungszeit hat.

```java
for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
      // Rumpf
    }
}
```

  * [ ] O(n)
  * [ ] O(n^2)
  * [ ] O(n^3)
  * [ ] O(n^4)
  * [ ] O(n^5)
  * [ ] O(log(n))
  * [ ] O(n log(n))

## 7.17 Komplexität bestimmen
Gegeben seien das folgenden Programmfragment. Geben Sie den Aufwand mittels der O-Notation an. Sie dürfen davon ausgehen, dass der fehlende Schleifenrumpf eine konstante Ausführungszeit hat.

```java
for (int i = 0; i < n; i++) {
    for (int j = 0; j < i; j++) {
        // Rumpf
    }
}
```

  * [ ] O(n)
  * [ ] O(n^2)
  * [ ] O(n^3)
  * [ ] O(n^4)
  * [ ] O(n^5)
  * [ ] O(log(n))
  * [ ] O(n log(n))

## 7.18 Komplexität bestimmen
Gegeben seien das folgenden Programmfragment. Geben Sie den Aufwand mittels der O-Notation an. Sie dürfen davon ausgehen, dass der fehlende Schleifenrumpf eine konstante Ausführungszeit hat.

```java
for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
        for (int k = 0; k < n; k++) {
           // Rumpf
        }
    }
}
```

  * [ ] O(n)
  * [ ] O(n^2)
  * [ ] O(n^3)
  * [ ] O(n^4)
  * [ ] O(n^5)
  * [ ] O(log(n))
  * [ ] O(n log(n))

## 7.19 Wörter tauschen
Geben Sie einen regulären Ausdruck an, der zwei durch Bindestrich (`-`) verbundene Wörter vertauscht. Z.B. soll aus "Speicher-Fehler" das Wort "Fehler-Speicher" werden. Orientieren Sie sich an der Syntax des Unix-Werkzeugs `sed` bei der Angabe des Ausdrucks (extended regular expressions mit der `-E`-Option).

  * [ ] `sed -E 's/.+-.+/\2-\1/g'`
  * [ ] `sed -E 's/[.+]-[.+]/\2-\1/g'`
  * [ ] `sed -E 's/(*)-(*)/\2-\1/g'`
  * [ ] `sed -E 's/(.+)-(.+)/\2-\1/g'`
  * [ ] `sed -E 's/(*)-(*)/$2-$1/g'`
  * [ ] `sed -E 's/.+-.+/$2-$1/g'`
  * [ ] `sed -E 's/[.+]-[.+]/$2-$1/g'`
  * [ ] `sed -E 's/(.+)-(.+)/$2-$1/g'`

## 7.20 Regulärer Ausdruck für Matrikelnummern
Geben Sie einen regulären Ausdruck an, der die Matrikelnummern der Studierenden, die im Sommersemester 2018 angefangen haben (beginnen mit `181` und darauf folgen immer vier Ziffern) matched. Andere, ähnliche Zahlen sollen nicht matchen.

  * [ ] `/181[09]*/`
  * [ ] `/^181(0-9)*$/`
  * [ ] `/181[0-9]*/`
  * [ ] `/^181[09]*$/`
  * [ ] `/^181[0-9]{4}$/`
  * [ ] `/181[0-9]{4}/`
  * [ ] `/^181[0-9]*$/`
  * [ ] `/^181[09]{4}$/`
  * [ ] `/181[09]{4}/`
  * [ ] `/181(0-9)*/`
  * [ ] `/181(0-9){4}/`
  * [ ] `/^181(0-9){4}$/`

## 7.21 Regulärer Ausdruck für Jahreszahlen
Geben Sie einen regulären Ausdruck an, der alle Jahreszahlen von 2000-2999 matched aber keine anderen Zahlen, z.B. `20` oder `22000`.

  * [ ] `/^2[0-9]{3}$/`
  * [ ] `/2[0-9]{3}/`
  * [ ] `/^2[0-9][0-9][0-9]$/`
  * [ ] `/^2.*$/`
  * [ ] `/^2.+$/`
  * [ ] `/2[0-9]{3}$/`

## 7.22 Erweiterte Backus-Naur-Form (EBNF)
Gegeben sei die folgende Grammatik in EBNF-Form

```console
expression = term  { ("+" | "-") term };
term       = factor  { ("*" | "/") factor };
factor     = constant | variable | "(" expression ")";
variable   = "x" | "y" | "z";
constant   = digit {digit} ;
digit      = "0" | "1" ... "9";
```

Welche der folgenden Ausdrücke erfüllen diese Grammatik?

  * [ ] `333 / z`
  * [ ] `(333 / z) + (4 - 6)`
  * [ ] `182 + x * x + z`
  * [ ] `182 * x + x * z`
  * [ ] `333 / c`
  * [ ] `x / y`
  * [ ] `a / b`
  * [ ] `182 * a + x * z`

## 7.23 Erweiterte Backus-Naur-Form (EBNF)
Gegeben sei die folgende Grammatik in EBNF-Form

```console
sign       = "+" | "-"
edigit     = "0" | "2" | "4" | "6" | "8"
digit      = edigit | "1" | "3" | "5" | "7" | "9"
number     = [sign]{digit}edigit
```

Welche der folgenden Ausdrücke erfüllen diese Grammatik?

  * [ ] `13`
  * [ ] `+3458`
  * [ ] `+37`
  * [ ] `3+4`
  * [ ] `+-3`
  * [ ] `digit`
  * [ ] `2`
  * [ ] `-56`
  * [ ] `2-3`
  * [ ] `-123`
  * [ ] `34`

