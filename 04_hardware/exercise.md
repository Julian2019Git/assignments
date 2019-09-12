# 4. Hardware - Übungen

## 4.1 PC konfigurieren
Stellen Sie zwei PCs zusammen, einmal einen mit maximaler Leistung für Computer-Spiele und einmal einen einfachen Rechner für das Surfen im Internet. Verwenden Sie keinen komplett PC, sondern stellen Sie die Geräte aus einzelnen Komponenten zusammen, die Sie im Internet bei einem Hardware-Versand (z.B. [Alternate](https://www.alternate.de)) finden. Stellen Sie eine Stückliste, inklusive Preisen zusammen. Was kosten die beiden Rechner?


## 4.2 Harvard-Architektur
Beschreiben Sie kurz den Aufbau einer _Harvard-Architektur_. In welchen Systemen findet man diese Architektur heute vor?


## 4.3 Von Neumann-Architektur
Beschreiben Sie kurz den Aufbau der _von Neumann-Architektur_. Welche fünf Funktionseinheiten hat die von Neumann Architektur?


## 4.4 Vergleich Harvard- mit von Neumann-Architektur
Vergleichen Sie kurz die Harvard mit der von Neumann-Architektur: Welche Vor- und Nachteile haben sie jeweils?


## 4.5 RISC vs. CISC
Stellen Sie kurz die Unterschiede zwischen einer CISC- und einer RISC-Architektur bei Prozessoren zusammen. Nennen Sie jeweils ein Beispiel für einen Prozessor mit RISC- bzw. CISC-Architektur. Haben moderne Intel-Prozessoren, z.B. der i7, eine RISC- oder CISC-Architektur? Wie verhält es sich mit dem Prozessor in heutigen Smartphones?


## 4.6 Prozessor
Aus welchen Einheiten besteht ein Prozessor und welche Funktion haben diese jeweils?


## 4.7 Register des Prozessors
Jeder Prozessor hat neben den "normalen" Registern einen Program Counter (PC) und ein Instruction Register (IR).

  1. Wie läuft die Ausführung von Befehlen ab?
  2. Wie werden Sprünge im Programm realisiert?


## 4.8 Adressraum
Wie viel Speicher in Kilobyte kann ein Computer adressieren, wenn seine Adressen 16 Bit lang sind?


## 4.9 64 Bit im Smartphone
Warum ist es für Smartphone-Nutzer wichtig, dass die Prozessoren im Smartphone in Zukunft auch 64 Bit-Architekturen sind?


## 4.10 GPU vs. CPU
Worin unterscheiden sich Grafikprozessoren (GPU) von "normalen" Prozessoren (CPU)? Beschreiben Sie die Unterschiede kurz.


## 4.11 SSDs -- Vorteile und Nachteile
Solid State Disks (SSDs) sind deutlich schneller als Festplatten (HDDs). Welche Gründe sprechen für und welche gegen eine SSD? Welche Anschlussmöglichkeiten gibt es für SSDs an den Rechner?


## 4.12 Rotationsgeschwindigkeit
Was gewinnt man, wenn man die Rotationsgeschwindigkeit einer Festplatte oder DVD erhöht?


## 4.13 Datenrate einer Festplatte
Angenommen die Festplatte in Ihrem PC dreht sich mit 5000 Umdrehungen pro Minute, jeder Track hat 16 Sektoren und jeder Sektor 1024 Byte. Welche Transferrate muss der Festplattencontroller unterstützen, um die Daten zu verarbeiten?


  * [ ] 0,3 MByte / Sekunde
  * [ ] 1,0 MByte / Sekunde
  * [ ] 1,3 MByte / Sekunde
  * [ ] 10,0 MByte / Sekunde
  * [ ] 20,4 MByte / Sekunde

## 4.14 Größe einer Textdatei
Manchmal verändert sich die Größe auf der Festplatte einer Textdatei beim Hinzufügen eines einzelnen Zeichens überhaupt nicht, ein anders Mal direkt um einige Hundert Bytes. Woran liegt das?


## 4.15 Leistung von USB-Ports
HD-Video hat eine Auflösung von 1920x1080 Pixel bei 30 Frames pro Sekunde mit 24 Bit pro Pixel. Kann man einen unkomprimierten HD-Video-Strom live über einen

  * USB 1.1-Port (12 MBit/s)
  * USB 2.0-Port (480 MBit/s)
  * USB 3.0-Port (5 GBit/s)

senden?


## 4.16 Datenrate einer Tastatur
Wie viele Bits pro Sekunde muss eine Tastatur übertragen, um mit einem Nutzer mitzuhalten, der 40 Worte pro Minute tippt?


## 4.17 Funktionseinheiten eines Prozessors
Bitte ordnen Sie die Funktionseinheiten eines Prozessors ihren jeweiligen Aufgaben zu:

  * ALU: ....
  * Control Unit: ....
  * Input Output Unit (IO-Unit): ....
  * Register: ....
  * Program Counter (PC): ....
  * Instruction Register (IR): ....
  * Cache: ....
  * Datenbus: ....
  * Adressbus: ....
  * Status Word: ....

*Antworten:*

  1. Verbindung zum Hauptspeicher
  2. Kommunikation mit dem Speicher
  3. schneller Speicher, um Zugriffe auf das RAM zu minimieren
  4. Zähler für den auszuführenden Befehl
  5. Ausgabe von Grafikdaten an den Bildschirm
  6. Speicher für Zwischenergebnisse bei Berechnungen
  7. Status, der von anderen Teilen des Prozessors erzeugt wird
  8. Durchführung von Berechnungen (Addition etc.)
  9. Ausführung von Maschinenbefehlen
  10. Steuerung des Massenspeichers
  11. Speicher für den aktuell auszuführenden Befehl


## 4.18 Vergleich Harvard- mit von Neumann-Architektur
Ordnen Sie der _Harvard_ bzw. _von Neumann-Architektur_ den entsprechenden Eigenschaften zu:

  * Findet sich hauptsächlich in Single-Chip-Microcontrollern: ....
  * Programmspeicher ist logisch und physisch vom Datenspeicher getrennt: ....
  * Höhere Durchsatz, da zwei getrennte Busse für Daten/Programme: ....
  * Ist Konstruktionsprinzip für moderne Desktopcomputer (PC): ....
  * Speicher kann besser genutzt werden (weniger Fragmentierung): ....
  * Gemeinsamer Speicher enthält sowohl Programme als auch Daten: ....
  * Schützt Programme vor Veränderungen: ....

*Antworten:*

  1. Harvard-Architektur
  2. von Neumann-Architektur


## 4.19 Register des Prozessors
Bitte bringen Sie die Schritte bei der Ausführung eines Befehls im Prozessor in die richtige Reihenfolge:

  * _write_: Ergebnisse zurück schreiben: ....
  * _fetch_: Nächste Instruktion aus dem Speicher in das Instruction Register laden: ....
  * _decode_: Instruktion im Register dekodieren: ....
  * _execute_: Instruktion ausführen: ....
  * _increment PC_: Programm Counter um eins erhöhen: ....
  * _fetch operands_: Operanden aus dem Speicher laden: ....

*Antworten:*

  1. Schritt 1
  2. Schritt 2
  3. Schritt 3
  4. Schritt 4
  5. Schritt 5
  6. Schritt 6


## 4.20 Speichertechnologie
Auf welcher Art von Speicher wird typischerweise welche Art / Technologie für die Speicherung von Daten verwendet?


  * Caches: ....
  * DVD: ....
  * Hauptspeicher: ....
  * Festplatte: ....
  * Blu-ray Disc: ....
  * DLT-Band: ....
  * SSD: ....
  * Register: ....

*Antworten:*

  1. SRAM
  2. Optische Datenträger
  3. Magnetische Datenträger
  4. Flash Speicherzellen
  5. DRAM
  6. SRAM oder DRAM


## 4.21 GPU vs. CPU
Worin unterscheiden sich Grafikprozessoren (GPU) von "normalen" Prozessoren (CPU)? Ordnen Sie entsprechend zu.

  * Einzelne Berechnung wird eher schnell ausgeführt: ....
  * Bestehen aus Shadern: ....
  * Viele parallele Berechnungen: ....
  * Besitzen eine begrenzte Anzahl von Recheneinheiten: ....
  * Bestehen aus Cores: ....
  * Besitzen sehr viele parallele Recheneinheiten: ....
  * Wenige parallele Berechnungen: ....
  * Einzelne Berechnung wird eher langsam ausgeführt: ....
  * Für generelle Anwendungen konzipiert: ....
  * Für Grafikanwendungen konzipiert: ....

*Antworten:*

  1. GPU
  2. CPU


## 4.22 RISC vs. CISC
Bitte ordnen Sie den beiden Architekturtypen für Prozessoren (RISC und CISC) die entsprechenden Eigenschaften zu:

  * Haben einen kleinen Dekodieraufwand für den einzelnen Befehl: ....
  * Haben einen eingeschränkten, einfachen Befehlssatz: ....
  * Haben einen großen Dekodieraufwand für den einzelnen Befehl: ....
  * ARM-Prozessoren (aus interner Sicht): ....
  * ARM-Prozessoren (aus Sicht des Programmierers): ....
  * Können einen einzelnen Befehl relativ langsam abarbeiten: ....
  * Haben einen umfangreichen, mächtigen Befehlssatz: ....
  * Können einen einzelnen Befehl relativ schnell abarbeiten: ....
  * Intel-Prozessoren (aus interner Sicht): ....
  * Intel-Prozessoren (aus Sicht des Programmierers): ....

*Antworten:*

  1. RISC
  2. CISC


## 4.23 Abkürzungen CISC und RISC
Wofür stehen die Abkürzungen CISC und RISC?

  * [ ] "Collaborative Intelligence and Science Collaboration" bzw. "Retarded Intelligence and Science Collaboration"
  * [ ] "Computing InfraStructure Compiler" bzw. "Risk InfraStructure Compiler"
  * [ ] es handelt sich nicht um Abkürzungen
  * [ ] "Complex Instruction Set Compiler" bzw. "Reduced Instruction Set Compiler"
  * [ ] "Complex Instruction Set Computer" bzw. "Reduced Instruction Set Computer"

## 4.24 SSDs -- Vorteile und Nachteile
Welche Aussagen treffen auf SSDs zu?

  * [ ] enthalten keine mechanischen Teile
  * [ ] haben eine deutlich höhere Lese- und Schreibgeschwindigkeit als Festplatten
  * [ ] haben konstruktionsbedingt weniger Speicherkapazität als Festplatten
  * [ ] unterliegen einem Verschleiß
  * [ ] sind resistent gegen Erschütterungen
  * [ ] speichern die Bits Flash-Zellen
  * [ ] speichern ihre Daten magnetisch
  * [ ] können per PCIe angeschlossen werden
  * [ ] haben dieselbe Speicherkapazität wie Festplatten
  * [ ] können nicht per SATA angeschlossen werden
  * [ ] verschleißen nie
  * [ ] können per m2 angeschlossen werden

## 4.25 Leistung von USB-Ports
HD-Video hat eine Auflösung von 1920x1080 Pixel bei 30 Frames pro Sekunde mit 24 Bit pro Pixel. Über welche Art von Port könnte man dieses Video live übertragen?


  * [ ] USB 1.0-Port (1.5 MBit/s)
  * [ ] USB 1.1-Port (12 MBit/s)
  * [ ] USB 2.0-Port (480 MBit/s)
  * [ ] USB 3.0-Port (5 GBit/s)
  * [ ] USB 3.1-Port (10 GBit/s)
  * [ ] USB 3.3-Port (20 GBit/s)

## 4.26 Leistung von USB-Ports
CD-Audio hat zwei Audio-Kanäle (Stereo) mit 16 Bit Auflösung und einer Sampling-Frequenz von 44,1 kHz. Über welche Art von Port könnte man einen solchen Audio-Strom live übertragen?


  * [ ] USB 1.0-Port (1.5 MBit/s)
  * [ ] USB 1.1-Port (12 MBit/s)
  * [ ] USB 2.0-Port (480 MBit/s)
  * [ ] USB 3.0-Port (5 GBit/s)
  * [ ] USB 3.1-Port (10 GBit/s)
  * [ ] USB 3.3-Port (20 GBit/s)

