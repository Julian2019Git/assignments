# 13. Künstliche Intelligenz - Übungen

## 13.1 Backpropagation
Was versteht man im Zusammenhang von Neuronalen Netzen unter _Backpropagation_?


## 13.2 Captcha
Heute müssen Internet-Benutzer häufig sogenannte Captchas lösen, um sich bei Webseiten anzumelden. In welchem Zusammenhang stehen Captchas zum Turing-Test?


## 13.3 Arten des maschinellen Lernens
Definieren Sie in kurzen Sätzen die folgenden Arten des maschinellen Lernens:

  1. Überwachtes Lernen (supervised learning)
  2. Unüberwachtes Lernen (unsupervised learning)
  3. Bestärkendes Lernen (reinforced learning)


## 13.4 Neuron
Ein künstliches Neuronales Netz besteht aus sogenannten _künstlichen Neuronen_. Erläutern Sie kurz, wie ein solches Neuron funktioniert.


## 13.5 Möglichkeiten und Grenzen der KI
Recherchieren Sie in der KI-Literatur bzw. im Internet, inwiefern folgende Probleme heutzutage mittels Computer- bzw. Robotereinsatz gelöst werden können:

  1. Spielen der Brettspiele Dame und Go
  2. Verarbeiten natürlicher Sprache in Echtzeit
  3. Autonomie unbemannter Fahr- und Flugzeuge (UGVs und UAVs)
  4. Automatische Gesichtserkennung
  5. Spielen von Computerspielen (z.B. klassische Atari-Spiele) wie ein Mensch.
  6. Komponieren von Musik.
  7. Turing-Test

Schreiben Sie Ihre Erkenntnisse in jeweils 2–3 Sätzen auf.


## 13.6 Schwache vs. Starke KI
Erläutern Sie den Unterschied zwischen einer _schwachen_ und einer _starken_ KI.


## 13.7 Turing Test
Erläutern Sie, was man unter dem Turing-Test versteht. Wann und wo wurde er erstmals beschrieben und wie läuft er ab?


## 13.8 Deep Learning
Was versteht man unter _Deep Learning_?


## 13.9 Robotergesetze
Isaac Asimov definierte in der Kurzgeschichte Runaround 1942 die drei sogenannten Robotergesetze. Wie lauten diese?


## 13.10 Superintelligenz
Definieren Sie kurz in eigenen Worten, was man unter einer _Superintelligenz_ versteht.


## 13.11 Typologie künstlicher Intelligenz
Man unterscheidet _vier Typen_ (oder Stufen) von künstlicher Intelligenz. Bitte erläutern Sie diese kurz.


## 13.12 Machine Learning: Begriffe
Bitte definieren Sie in Ihren eigenen Worten kurz die folgenden zentralen Begriffe aus dem Machine Learning:

  1. Features
  2. Klassifikation (classification)
  3. Trainingsdaten (training data)
  4. Label
  5. Labeled Data / Unlabeled Data
  6. Decision Boundaries
  7. Entscheidungsbaum (decision tree)
  8. Forest
  9. Confusion Matrix


## 13.13 Entscheidungsbaum erstellen
Gegeben sind Messwerte für das Gewicht und den Durchmesser von Mandarinen, Orangen und Zitronen, die als CSV-Dateien vorliegen:

  1. Mandarinen: [mandarine.csv](data/mandarine.csv)
  2. Orangen: [orange.csv](data/orange.csv)
  3. Zitrone: [zitrone.csv](data/zitrone.csv)

Zeichnen Sie die Daten in einem Diagramm und definieren Sie dann basierend darauf einen Classifier in Form eines Entscheidungsbaum, der aufgrund von Gewicht und Größe die Daten den drei Klassen "Mandarine", "Orange" oder "Zitrone" zuordnet.

Tipp: Die Daten lassen sich sehr leicht mit dem Werkzeug [GNUPlot](http://www.gnuplot.info) in einem Diagramm ausgeben.

Wie Objekte (Obststücke) aus den Beispieldateien werden durch Ihren Classifier richtig, wie viele falsch klassifiziert?

Sie finden ein unbekanntes Objekt in einem Obstkorb, mit einer Masse von 140g und einem Durchmesser von 6cm. Um was handelt es sich Ihrer Meinung nach?


## 13.14 Berechnungen an einem Neuron
Gegeben sei ein künstliches Neuron mit drei Eingängen (x1, x2 und x3) (und einem Ausgang a). Die Gewichte für die drei Eingänge sind:

  * w1: 0.3
  * w2: 0.5
  * w3: 0.2

Als Aktivierungsfunktion wird die Sigmoid-Funktion verwendet, wobei vorher noch ein Bias addiert wird. Der Bias beträgt konstant -2.0. Den Verlauf der Sigmoid-Funktion `f(x) = 1 / (1 + exp(-x))` für das Neuron können Sie aus folgender Grafik ableiten:

![](img/sigmoid.png)

Berechnen Sie für folgende Werte die Ausgabe des Neurons:

(x1, x2, x3) = (4.3, 2.6, 2.0)


## 13.15 Berechnungen an einem Neuron
Gegeben sei ein künstliches Neuron mit drei Eingängen (x1, x2 und x3) (und einem Ausgang a). Die Gewichte für die drei Eingänge sind:

  * w1: 0.3
  * w2: 0.5
  * w3: 0.2

Als Aktivierungsfunktion wird die Sigmoid-Funktion verwendet, wobei vorher noch ein Bias addiert wird. Der Bias beträgt konstant -2.0. Den Verlauf der Sigmoid-Funktion `f(x) = 1 / (1 + exp(-x))` für das Neuron können Sie aus folgender Grafik ableiten:

![](img/sigmoid.png)

Berechnen Sie für folgende Werte die Ausgabe des Neurons:

(x1, x2, x3) = (1.3, -4.8, -1.9)


