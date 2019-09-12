# 8. Netzwerke - Übungen

## 8.1 Datentransferrate
Wie lange braucht man, um einen Roman mit 300 Seiten, codiert in Unicode (UCS2) bei einer Datentransferrate von 54 Mbit/s zu übertragen?


## 8.2 MAC-Adresse
Wieso hat die Netzwerkkarte in Ihrem Rechner zusätzlich zur IP-Adresse auch noch eine MAC-Adresse? Wie hängen die beiden zusammen? 


## 8.3 MAC statt IP
Angenommen, es hätte das Ethernet-Protokoll schon zu der Zeit gegeben, als das Internet entwickelt wurde: Hätte es nicht gereicht, einfach die MAC-Adresse zu verwenden und ganz auf die IP zu verzichten?


## 8.4 Adressknappheit
Warum sind die IPv4-Adressen inzwischen sehr knapp geworden?


## 8.5 NAT
Wieso hat die Einführung von *NAT* die Knappheit bei den IPv4-Adressen etwas gemildert?


## 8.6 Spezielle Adressen
Was ist das Besondere an den IP-Adressen `192.168.*.*`, `10.*.*.*`, `127.0.0.1`?


## 8.7 Hidden-Station-Problem
Was ist das Hidden-Station-Problem, auch Hidden-Node-Problem genannt?


## 8.8 CSMA/CD im WLAN
Warum kann man das CSMA/CD-Protokoll nicht in einem WLAN verwenden?


## 8.9 IPv6 Adressraum
IPv4 benutzt 32-Bit-Adressen, die inzwischen nicht mehr ausreichen, um alle Geräte im Internet zu adressieren. IPv6 setzt 128-Bit-Adressen ein. Ist dies diesmal ausreichend oder wird es in der Zukunft wieder zu Knappheit der Adressen kommen? Begründen Sie Ihre Antwort.


## 8.10 Bridge vs. Router vs. Switch
Erläutern Sie bitte kurz die Unterschiede zwischen einer Bridge, einem Router und einem Switch.


## 8.11 Hub oder Switch
Wenn Sie die Wahl hätten, einen Hub oder einen Switch einzusetzen, welche Komponente würden Sie (unter der Annahme gleicher Kosten) einsetzen? Begründen Sie Ihre Antwort kurz.


## 8.12 Fehlerkorrektur in UDP
Mit welchem Verfahren behandelt UDP das Auftreten eines Fehlers? Was ist der Unterschied zwischen UDP und TCP?


## 8.13 ARP
Um ein IP-Paket zustellen zu können, muss der Router die IP-Adresse zu der MAC-Adresse des Ziel-Hosts auflösen. Hierzu wird das *Address Resolution Protocol (ARP)* verwendet. Beschreiben Sie bitte grob, wie eine solche Auflösung abläuft.


## 8.14 Unicast / Multicast / Braodcast
Man unterscheidet im Rahmen von Netzwerken zwischen *Unicast*, *Broadcast* und *Multicast*. Bitte erläutern Sie was diese Begriffe bezeichnen und worin die Unterschiede bestehen. Geben Sie jeweils ein Beispiel.


## 8.15 Netzmaske
Im Rahmen des Internet Protocols Version 4 (IPv4) taucht immer wieder die sogenannte __Netzmaske__ auf. Beschreiben Sie bitten welchem Zweck die Netzmaske dient, wie sie aufgebaut ist und wie man sie notieren kann.


## 8.16 Routing
Eine wichtige Eigenschaft des Internets ist das sogenannte __Routing__. Erläutern Sie bitte kurz, was sich hinter dem Begriff Routing verbirgt.


## 8.17 Dynamisches Routing
Erläutern Sie bitte kurz, warum ein paktvermitteltes Netz eine Grundvoraussetzung für das dynamische Routing von Daten im Netzwerk ist.


## 8.18 Ports
Sowohl TCP als auch UDP verwenden sogenannte __Ports__. Erläutern Sie bitte, welchem Zweck die Ports bei TCP und UDP dienen. Geben Sie Ihnen bekannte Ports an.


## 8.19 Verbindung in TCP
Das __Transmission Control Protocol (TCP)__ ist verbindungsorientiert und zuverlässig. Erläutern Sie bitte, wie es TCP gelingt eine Verbindung und die Zuverlässigkeit der Kommunikation auf Grundlage des paketvermittelten IP-Protokolls zu realisieren.


## 8.20 DHCP
Ein wichtiges Protokoll im Rahmen des Internet ist *DHCP*. Beschreiben Sie bitte kurz, um was es sich bei DHCP handelt und wie das Protokoll funktioniert.


## 8.21 Aufgaben von Protokollen
Bitte ordnen Sie den Protokollen/Technologien ihre jeweilige Aufgabe zu:

  * ARP: ....
  * DHCP: ....
  * NAT: ....
  * UDP: ....
  * TCP: ....
  * CIDR: ....

*Antworten:*

  1. IP-Adresse zu der MAC-Adresse auflösen
  2. IP-Adressen dynamisch den Hosts zuteilen
  3. mehrere Rechner in einem Netz hinter einer einzigen IP-Adresse verbergen
  4. Verbindungslose Übertragung von einzelnen Datenpaketen ohne Fehlerkorrektur
  5. Verbindungsorientierte Übertragung von Daten mit Fehlerkorrektur
  6. Festlegung von Netzwerk- und Host-Teil einer IP-Adresse basierend auf der Netzmaske


## 8.22 ARP
Um ein IP-Paket zustellen zu können, muss der Router die IP-Adresse zu der MAC-Adresse des Ziel-Hosts auflösen. Hierzu wird das *Address Resolution Protocol (ARP)* verwendet. Bringen Sie die Schritte der Auflösung in die richtige Reihenfolge.

  * Schritt 1: ....
  * Schritt 2: ....
  * Schritt 3: ....
  * Schritt 4: ....

*Antworten:*

  1. Broadcast im LAN an ff:ff:ff:ff:ff:ff fragt nach Rechner mit passender IP-Adresse
  2. Rechner mit der IP-Adresse antwortet mit seiner MAC-Adresse
  3. Router speichert die Zuordnung (cache) für eine gewisse Zeit
  4. Router kann dann das Paket dorthin ausliefern


## 8.23 Bridge vs. Router vs. Switch
Ordnen Sie die folgenden Eigenschaften den jeweiligen Geräten (Bridge, Router, Switch) zu:

  * Verbindet zwei Netzwerksegmente und arbeitet auf OSI-Level 2: ....
  * Hat in jedem Subnetz ein Interface mit MAC- und IP-Adresse: ....
  * Arbeitet auf der Sicherungsschicht: ....
  * Verteilt die Ethernet-Pakete an die einzelnen Hosts: ....
  * Arbeitet auf der Vermittlungsschicht: ....
  * Arbeitet in einem Netzwerksegment: ....
  * Verbindet verschiedene Subnetze miteinander: ....

*Antworten:*

  1. Bridge
  2. Router
  3. Switch


## 8.24 Datentransferrate
Wie lange braucht man ungefähr, um einen Roman mit 300 Seiten (30 Zeile mit 60 Zeichen), codiert in Unicode (UCS2) bei einer Datentransferrate von 54 Mbit/s zu übertragen?


  * [ ] 50 Millisekunden
  * [ ] 150 Millisekunden
  * [ ] 250 Millisekunden
  * [ ] 350 Millisekunden
  * [ ] 1 Sekunde
  * [ ] 5 Sekunden

## 8.25 Hidden-Station-Problem
Was ist das Hidden-Station-Problem, auch Hidden-Node-Problem genannt?

  * [ ] Eine Station versteckt sich absichtlich vor anderen
  * [ ] Eine Station ist vor allen Teilnehmern und dem Access-Point (AP) verborgen
  * [ ] Der Access-Point (AP) sieht eine Station, andere Teilnehmer im Netz können sie nicht sehen
  * [ ] Eine Station sieht weder die anderen Teilnehmer, noch den Access-Point (AP)

## 8.26 Bitbreite von IPv4- und IPv6-Adressen
Wie breit (in Bit) ist eine IPv4- bzw. eine IPv6-Adresse?

  * IPv6: ....
  * IPv4: ....

*Antworten:*

  1. 16 Bit
  2. 32 Bit
  3. 64 Bit
  4. 128 Bit
  5. 256 Bit
  6. 1024 Bit


## 8.27 Uni-, Multi- und Broadcast
Bitte ordnen Sie die Definitionen den richtigen Begriffen zu:

  * Datenpakete werden an alle Hosts in einem Netz geschickt: ....
  * Datenpakete werden an genau einen Host geschickt: ....
  * Datenpakete werden an mehrere Hosts in einem Netz geschickt: ....

*Antworten:*

  1. Unicast
  2. Multicast
  3. Broadcast


## 8.28 Netzmaske berechnen
Gegeben sei ein IPv4-Netz mit einer /12-Netzmaske. Bestimmen Sie bitte für die IP-Adresse `173.194.69.102` die Netz-Adresse.


  * [ ] `173.192.69.0`
  * [ ] `173.192.0.0`
  * [ ] `173.192.16.0`
  * [ ] `173.190.0.0`
  * [ ] `173.192.69.8`

## 8.29 Netzmaske berechnen
Gegeben sei ein IPv4-Netz mit einer /16-Netzmaske. Bestimmen Sie bitte für die IP-Adresse `8.8.19.240` die Netz-Adresse.

  * [ ] `8.8.0.0`
  * [ ] `8.8.19.240`
  * [ ] `8.8.19.0`
  * [ ] `8.0.0.0`
  * [ ] `8.8.19.32`
  * [ ] `8.8.12.0`

## 8.30 TCP vs. UDP
Welche Unterschiede gibt es zwischen TCP und UDP? Ordnen Sie passend zu:

  * verbindungsorientiert: ....
  * zuverlässig: ....
  * paketorientiert: ....
  * unzuverlässig: ....
  * Fehlerkorrektur ist Sache des Programmierers: ....
  * Fehlerkorrektur wird vom Protokoll übernommen: ....
  * Verbindung besteht, bis sie geschlossen wird: ....
  * Datenpakete haben eine Sequenznummer: ....

*Antworten:*

  1. TCP
  2. UDP


## 8.31 Anhängsel an URL
Worum handelt es sich bei dem Anhängsel an der URL (die Zahl nach dem Doppelpunkt), z.B. `http://joe.cs.hs-mannheim.de:8080`?

  * [ ] Subdomain
  * [ ] Pfad
  * [ ] Benutzername
  * [ ] Port
  * [ ] Timeout
  * [ ] IP-Suffix

## 8.32 Arten von Adressen
Bitte ordnen Sie die Begriffe und Definitionen korrekt zu:

  * sind 32 oder 128 Bit breit: ....
  * kann geroutet werden: ....
  * ist dem Network-Layer zuzuordnen: ....
  * sind 48 Bit breit: ....
  * sind hierarchisch aufgebaut: ....
  * ist dem Data Link Layer zuzuordnen: ....
  * ist spezifisch für das Ethernet-Protokoll: ....
  * dient der eindeutigen Identifikation im Internet: ....
  * unterstützt kein Routing: ....
  * sind flach aufgebaut: ....

*Antworten:*

  1. IP-Adresse
  2. MAC-Adresse
  3. UDP-Adresse
  4. ARP-Adresse
  5. TCP-Adresse


## 8.33 Hub oder Switch
Ordnen Sie die Eigenschaften passend zu:


  * vermeidet Netzwerkkollisionen: ....
  * ist unsicherer: ....
  * sendet die Datenpakete an alle Ports: ....
  * sendet die Datenpakete nur an einen Port: ....
  * ist sicherer: ....

*Antworten:*

  1. Hub
  2. Switch


