# 6. Betriebssysteme - Übungen

Für die Ausführung einiger dieser Übungen benötigen Sie ein funktionierendes Linux-System. Hierzu können Sie entweder

  * Ein eigenes Linux in einer virtuellen Maschine installieren (z.B. [VirtualBox](https://www.virtualbox.org) mit [Ubuntu](www.ubuntu.com))
  * Ein Live-Linux auf Ihrem Rechner starten, z.B. [Slax](http://www.slax.org)
  * An der Hochschule in einem der Poolräume eine Linux-VM starten
  * Sich mit Ihrem Fakultätsaccount auf `jonathan.sv.hs-mannheim.de` anmelden
  * Unter Android die Terminal-Emulation [Termux](https://play.google.com/store/apps/details?id=com.termux) installieren


## 6.1 Betriebssystem
Was versteht man unter einem Betriebssystem, und was sind dessen zentrale Aufgaben? Welche Betriebssysteme kennen Sie?


## 6.2 Betriebssystem auf Ihrem Smartphone
Welches Betriebssystem befindet sich auf Ihrem Smartphone? Von welchem Betriebssystem stammt es ab?


*Antworten:*



## 6.3 Prozess vs. Programm
Erläutern Sie den Unterschied zwischen einem __Prozess__ und eine __Programm__.


## 6.4 Auf jonathan anmelden
Um auf den Rechner `jonathan.sv.hs-mannheim.de` zugreifen zu können, benötigen Sie einen ssh-Client

  * Windows: [PuTTY](https://putty.org)
  * Mac: ssh-Client ist eingebaut
  * Linux: ssh-Client ist eingebaut
  * Android: [JuiceSSH](https://play.google.com/store/apps/details?id=com.sonelli.juicessh)

Nachdem Sie den Client installiert haben, loggen Sie sich auf `jonathan.sv.hs-mannheim.de` mit Ihrem Fakultätsaccount ein.

Finden Sie heraus, welchen Inhalt die Datei `/etc/exports` hat und geben Sie die ersten 10 Zeilen an.


## 6.5 Hilfe holen
Öffnen Sie auf einem Rechner mit dem Betriebssystem Linux eine Shell (Terminal). Verwenden Sie das Kommando `man`, um sich die Hilfe zum Kommando `ls` anzusehen. Welche Aufgabe hat die Option `-h` beim Kommando `ls`?


  * [ ] Zeigt den Inhalt das Hauptverzeichnisses an
  * [ ] Zeigt die Hilfeseite für das Kommando an
  * [ ] Zeigt die Größen mit zusätzlichen Einheiten an

## 6.6 Verzeichnisse
Öffnen Sie auf einem Rechner mit dem Betriebssystem Linux eine Shell (Terminal).

  1. Was ist Ihr aktuelles Arbeitsverzeichnis?
  2. Wie können Sie das aktuelle Verzeichnis herausfinden?
  3. Wechseln Sie mit der Shell zum Wurzelverzeichnis (`cd`) und zeigen dort alle Dateien und Verzeichnisse an (`ls`).
  4. Wem gehören die Dateien und Verzeichnisse im Wurzelverzeichnis? Wem in Ihrem Arbeitsverzeichnis?

Schauen Sie sich ein wenig auf dem System um. Was fällt Ihnen auf? Welche Verzeichnisse und Dateien sehen Sie? Was fällt Ihnen auf?


## 6.7 Verzeichnisse und Dateien anlegen/löschen
Öffnen Sie auf einem Rechner mit dem Betriebssystem Linux eine Shell (Terminal).

  1. Legen Sie ein Verzeichnis an (`mkdir`)
  2. Wechseln Sie in das Verzeichnis (`cd`)
  3. Erzeugen Sie im Verzeichnis eine Datei mit einem beliebigen Namen (`touch`)
  4. Verlassen Sie das Verzeichnis (`cd`)
  5. Versuchen Sie das Verzeichnis zu löschen (`rmdir`)

Was passiert? Was müssen Sie tun, um das Verzeichnis zu löschen?


## 6.8 Dateien kopieren/verschieben
Öffnen Sie auf einem Rechner mit dem Betriebssystem Linux eine Shell (Terminal).

  1. Legen Sie ein Verzeichnis an (`mkdir`)
  2. Wechseln Sie in das Verzeichnis (`cd`)
  3. Erzeugen Sie im Verzeichnis eine Datei mit einem beliebigen Namen und schreiben Sie einen Text in die Datei (`nano` oder `vi`)
  4. Kopieren Sie die Datei (`cp`)
  5. Editieren Sie die kopierte Datei (`nano` oder `vi`)
  6. Vergleichen Sie beide Dateien miteinander (`diff`)

Was sehen Sie?

  7. Legen Sie ein weiteres Verzeichnis an (`mkdir`)
  8. Verschieben Sie eine der beiden Dateien in das neue Verzeichnis (`mv`)


## 6.9 Weitere Unix-Kommandos
Schauen Sie sich die Hilfeseiten (oder das Buch "The Linux Command Line") zu den folgenden Kommandos an und geben Sie zu jedem kurz (in einem Satz) dessen Aufgabe an.

  1. `file`
  2. `less`
  3. `cat`
  4. `ln`
  5. `which`
  6. `whoami`
  7. `sort`
  8. `uniq`
  9. `grep`
  10. `head`
  11. `tail`
  12. `wc`
  13. `echo`
  14. `clear`
  15. `history`
  16. `sed`
  17. `du`
  18. `df`


## 6.10 Spezielle Verzeichnisse
Öffnen Sie auf einem Rechner mit dem Betriebssystem Linux eine Shell (Terminal). Schauen Sie sich auf der Festplatte ein wenig um, indem Sie mit `cd` durch die Verzeichnisse gehen und sich deren Inhalt mit `ls` anzeigen lassen.

Wozu dienen die folgenden Verzeichnisse:

  1. `/etc`
  2. `/dev`
  3. `/bin`
  4. `/home`
  5. `/tmp`


## 6.11 Berechtigungen
Sie sehen in einem Verzeichnis den folgenden Eintrag:

```console
-rw-rw-r--   1 thomas  staff   6,1K 28 Sep  2017 datei.txt
```

Was können Sie über die Berechtigungen dieser Datei sagen?

<div style="border: 1px solid grey;"><br><br><br><br><br><br><br><br></div>


## 6.12 Berechtigungen
Öffnen Sie auf einem Rechner mit dem Betriebssystem Linux eine Shell (Terminal). Schauen Sie sich die Hilfeseiten (oder das Buch "The Linux Command Line") zu den folgenden Kommandos an und experimentieren Sie damit ein wenig.

  1. `chmod`
  2. `chown`
  3. `chgrp`
  4. `passwd`
  5. `sudo`
  6. `su`

Keine Abgabe nötig! Ihr Wissen wird dann vor Ort geprüft.

## 6.13 Prozesse
Öffnen Sie auf einem Rechner mit dem Betriebssystem Linux eine Shell (Terminal). Schauen Sie sich die Hilfeseiten (oder das Buch "The Linux Command Line") zu den folgenden Kommandos an und experimentieren Sie damit ein wenig.

  1. `ps`
  2. `top`
  3. `kill`
  4. `killall`
  5. `shutdown`

Keine Abgabe nötig! Ihr Wissen wird dann vor Ort geprüft.

## 6.14 Eingabe- und Ausgabeumlenkung
Öffnen Sie auf einem Rechner mit dem Betriebssystem Linux eine Shell (Terminal). Experimentieren Sie mit der Eingabe-/Ausgabeumlenkung (`>`, `<`) und Pipes (`|`). Siehe hierzu Kapitel 6 in "The Linux Command Line".

Was ist der Unterschied zwischen `>`/`<` und `|`?


## 6.15 Betriebssysteme Grundlagen
Wofür steht die Abkürzung _HAL_ im Zusammenhang mit Betriebssystemen?


## 6.16 Betriebssysteme Architektur
Wie nennt man den Teil des Betriebssystems, der im privilegierten Modus läuft?


## 6.17 CPU-Vergabe
Wie nennt man den Vorgang in einem Betriebssystem, der für die Zuordnung der CPU(s) zu den abzuarbeitenden Prozessen zuständig ist?

  * [ ] kritischer Bereich
  * [ ] Mutual Exclusion
  * [ ] work plan
  * [ ] Scheduling

## 6.18 Threads
Was ist ein Thread aus Sicht des Betriebssystems?

  * [ ] eine Folge von Befehlen aus unterschiedlichen Programmen, jeweils 1 Befehl pro Programm
  * [ ] die Menge aller gleichzeitig ausführbaren Befehle eines Programms
  * [ ] eine Menge von beliebigen auszuführenden Befehlen unterschiedlicher Programme
  * [ ] eine Folge von sequentiell auszuführenden Befehlen innerhalb eines Programms
  * [ ] eine Menge parallel ausführbarer Programme

## 6.19 Hilfe holen
Wie können Sie sich die Hilfeseiten zum Kommando `sort` anzeigen lassen?

  * [ ] `cat sort`
  * [ ] `man sort`
  * [ ] `support sort`
  * [ ] `sort -help`
  * [ ] `ls sort`
  * [ ] `sort -h`
  * [ ] `help sort`
  * [ ] `less sort`

## 6.20 Berechtigungen
Sie sehen in einem Verzeichnis den folgenden Eintrag:

```console
-rw-rw-r--   1 thomas  staff   6,1K 28 Sep  2019 datei
```

Was können Sie über die Berechtigungen dieser Datei sagen?

  * [ ] Die Datei gehört dem Benutzer `thomas`
  * [ ] Jeder beliebige Benutzer darf die Datei schreiben
  * [ ] Die Gruppe darf die Datei ausführen
  * [ ] Die Datei gehört der Gruppe `thomas`
  * [ ] Jeder beliebige Benutzer darf die Datei ausführen
  * [ ] Die Gruppe darf die Datei schreiben
  * [ ] Die Datei gehört dem Benutzer `staff`
  * [ ] Der Benutzer darf die Datei ausführen
  * [ ] Die Gruppe darf die Datei lesen
  * [ ] Der Benutzer darf die Datei schreiben
  * [ ] Jeder beliebige Benutzer darf die Datei lesen
  * [ ] Der Benutzer darf die Datei lesen
  * [ ] Die Datei gehört der Gruppe `staff`

## 6.21 Berechtigungen
Sie sehen in einem Verzeichnis den folgenden Eintrag:

```console
-rwxr-x---   1 thomas  staff   6,1K 28 Sep  2019 datei
```

Was können Sie über die Berechtigungen dieser Datei sagen?

  * [ ] Die Gruppe darf die Datei schreiben
  * [ ] Die Gruppe darf die Datei lesen
  * [ ] Der Benutzer darf die Datei lesen
  * [ ] Die Datei gehört dem Benutzer `thomas`
  * [ ] Der Benutzer darf die Datei ausführen
  * [ ] Der Benutzer darf die Datei schreiben
  * [ ] Die Datei gehört der Gruppe `staff`
  * [ ] Jeder beliebige Benutzer darf die Datei ausführen
  * [ ] Jeder beliebige Benutzer darf die Datei lesen
  * [ ] Die Datei gehört der Gruppe `thomas`
  * [ ] Jeder beliebige Benutzer darf die Datei schreiben
  * [ ] Die Datei gehört dem Benutzer `staff`
  * [ ] Die Gruppe darf die Datei ausführen

## 6.22 Unix-Kommandos
Bitte ordnen Sie den Unix-Kommandos ihre jeweilige Aufgabe zu:


  * `cat`: ....
  * `cd`: ....
  * `chgrp`: ....
  * `chmod`: ....
  * `chown`: ....
  * `clear`: ....
  * `cp`: ....
  * `df`: ....
  * `diff`: ....
  * `du`: ....
  * `echo`: ....
  * `find`: ....
  * `grep`: ....
  * `head`: ....
  * `history`: ....
  * `kill`: ....
  * `less`: ....
  * `ln`: ....
  * `ls`: ....
  * `man`: ....
  * `mkdir`: ....

*Antworten:*

  1. In ein anderes Verzeichnis wechseln
  2. Die Gruppenzugehörigkeit einer Datei ändern
  3. Eine Prozess beenden
  4. Hilfeseiten aufrufen
  5. Den Anfang einer Datei ausgeben
  6. Einen Link erstellen
  7. Inhalt einer Datei ausgeben
  8. Freien Plattenplatz anzeigen
  9. Eine Datei kopieren
  10. Einen Text ausgeben
  11. Benutzen Plattenplatz anzeigen
  12. Die letzten, eingegeben Befehle ausgeben
  13. Zwei Dateien miteinander vergleichen
  14. Ein Verzeichnis anlegen
  15. Dateien mit einem bestimmten Namen finden
  16. Den Verzeichnisinhalt anzeigen
  17. Den Bildschirm löschen
  18. Dateien nach einem bestimmten Inhalt untersuchen
  19. Die Zugriffsrechte einer Datei anpassen
  20. Den Besitzer einer Datei ändenr


## 6.23 Unix-Kommandos
Bitte ordnen Sie den Unix-Kommandos ihre jeweilige Aufgabe zu:

  * `more`: ....
  * `mv`: ....
  * `passwd`: ....
  * `ping`: ....
  * `ps`: ....
  * `pwd`: ....
  * `reboot`: ....
  * `rm`: ....
  * `rmdir`: ....
  * `sed`: ....
  * `shutdown`: ....
  * `sort`: ....
  * `ssh`: ....
  * `su`: ....
  * `sudo`: ....
  * `tail`: ....
  * `top`: ....
  * `uniq`: ....
  * `vi`: ....
  * `wc`: ....
  * `which`: ....

*Antworten:*

  1. Dateien löschen
  2. Sich an einem anderen Computer anmelden
  3. Das Ende einer Datei anzeigen
  4. Den Computer neu starten
  5. Ein Verzeichnis löschen
  6. Das folgende Kommando als root ausführen
  7. Prüfen, ob ein Rechner über das Internet erreichbar ist
  8. Laufende Prozesse anzeigen
  9. Den Computer herunterfahren
  10. Ersetzungen mit regulären Ausdrücken durchführen
  11. Texte editieren
  12. Anzeigen, welchen Pfad ein Kommando hat
  13. Doubletten entfernen
  14. Das aktuelle Verzeichnis ausgeben
  15. Worte und Zeilen zählen
  16. Den Benutzer wechseln
  17. Inhalte sortieren
  18. Das Passwort ändern
  19. Inhalt einer Datei ausgeben
  20. Eine Datei verschieben oder umbenennen


## 6.24 Eingabe- und Ausgabeumlenkung
Sie wollen den Inhalt einer Datei `names.txt` sortieren und danach alle doppelten Einträge entfernen. Das Ergebnis soll in eine neue Datei `result.txt` geschrieben werden. Welche Kommandos sind hierfür korrekt?

  * [ ] sort < names.txt | uniq | result.txt
  * [ ] sort names.txt | uniq < result.txt
  * [ ] sort names.txt | uniq > result.txt
  * [ ] cat names.txt | sort | uniq < result.txt
  * [ ] sort < names.txt | uniq < result.txt
  * [ ] cat names.txt | sort | uniq | result.txt
  * [ ] sort < names.txt | uniq > result.txt
  * [ ] sort names.txt | uniq | result.txt
  * [ ] sort names.txt > uniq > result.txt
  * [ ] names.txt | sort | uniq > result.txt
  * [ ] cat names.txt | sort | uniq > result.txt
  * [ ] cat names.txt > sort > uniq > result.txt

## 6.25 Spezielle Verzeichnisse
Ordnen Sie bitte den angegebenen Verzeichnissen ihre jeweilige Rolle in einem Unix-System zu:

  * `/etc`: ....
  * `/dev`: ....
  * `/bin`: ....
  * `/sbin`: ....
  * `/home`: ....
  * `/tmp`: ....
  * `/proc`: ....
  * `/var`: ....
  * `/root`: ....

*Antworten:*

  1. Daten des privilegierten Benutzers
  2. Dateien des Systems, die sich ständig ändern
  3. Ausführbare Programme
  4. Konfigurationsdateien
  5. Temporäre Dateien
  6. Laufzeitinformationen zum Betriebssystem
  7. Gerätedateien
  8. Daten der Benutzer


## 6.26 Prozess vs. Programm
Ordnen Sie __Prozess__ und __Programm__ die jeweiligen Eigenschaften zu.

  * Führt exakt ein P. aus: ....
  * Auf der Festplatte gespeichert: ....
  * Ein P., das gerade ausgeführt wird: ....
  * Arbeitseinheit des Betriebssystems: ....
  * Passive Entität: ....
  * Ist isoliert von anderen: ....
  * Wird in den Speicher geladen: ....
  * Kann mehrfach ausgeführt werden: ....

*Antworten:*

  1. Prozess
  2. Programm


## 6.27 Komponenten eines Betriebssystems
Ordnen Sie den unten genannten Aufgaben die jeweiligen Komponenten des Betriebssystems zu, die für diese Aufgaben zuständig sind:

  * Kommunikation zwischen Prozessen ermöglichen: ....
  * Programmen Dienste des Betriebssystems zur Verfügung stellen: ....
  * Dateien verwalten, anlegen, löschen etc.: ....
  * Rechenzeit an Prozesse verteilen: ....
  * Benutzereingaben auf der Konsole annehmen und ausführen: ....
  * Physischen und logischen Speicher trennen: ....
  * Rechenzeit an Threads verteilen: ....

*Antworten:*

  1. System-Calls
  2. IPC (Inter-process communication)
  3. Shell
  4. Virtual Memory
  5. Scheduler
  6. Dateisystem


