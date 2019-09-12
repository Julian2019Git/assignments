# 9. WWW und Internet - Übungen

## 9.1 C/S-Modell vs. P2P
Vergleichen Sie Client/Server-Modell mit dem Peer-to-Peer-Modell. Geben Sie Beispiele für die beiden Modelle.


## 9.2 DNS
Wie funktioniert die Auflösung einer Adresse (z.B. `www.google.com`) in die IP-Adresse? Wo kommt das DNS ins Spiel?


## 9.3 Mail-Protokolle
Wieso gibt es für den Umgang mit E-Mails drei Protokoll (SMTP, POP3, IMAP)?


## 9.4 HTTPS
Was ist der Unterschied zwischen dem Zugriff auf die URL `http://stargazer.universe.org` und `https://stargazer.universe.org`?

  * [ ] Der Zugriff auf den Server mit der `http`-URL erfolgt über einen Proxy
  * [ ] Der Zugriff auf den Server mit der `https`-URL erfolgt über einen Proxy
  * [ ] Es sind keine gültigen URLs
  * [ ] Der Zugriff auf den Server mit der `http`-URL erfolgt verschlüsselt
  * [ ] Der Zugriff auf den Server mit der `https`-URL erfolgt verschlüsselt

## 9.5 HTTPS
Welche Aussagen über HTTPS sind korrekt?

  * [ ] es basiert auf SSH
  * [ ] der Browser kann sich gegenüber dem Server identifizieren
  * [ ] es verwendet PGP-Keys
  * [ ] der Server identifiziert sich gegenüber dem Browser
  * [ ] die Speicherung der Daten erfolgt verschlüsselt
  * [ ] es basiert auf SSL/TLS
  * [ ] die Kommunikation erfolgt verschlüsselt
  * [ ] es verwendet Zertifikate
  * [ ] es verschlüsselt die Daten asymmetrisch

## 9.6 HTML-Struktur
Öffnen Sie eine Webseite und schauen Sie sich den Quelltext der HTML-Datei an. Welche grundlegende Struktur können Sie erkennen?


## 9.7 HTML-Seite erstellen
Erstellen Sie eine einfache HTML-Seite, in der Sie Ihren Lieblingsfilm vorstellen. Verwenden Sie auf jeden Fall Bilder, um die Seite ansprechender zu gestalten. Verwenden Sie CSS, um die Seite optisch zu gestalten.

Legen Sie die Seite auf dem Rechner `jonathan.sv.hs-mannheim.de` im Verzeichnis `public_html` (falls nicht vorhanden, müssen Sie das Verzeichnis anlegen) unter dem Namen `index.html` ab. Sie können die Seite dann unter `http://jonathan.sv.hs-mannheim.de/~NUTZERNAME/` über das Internet abrufen, wobei NUTZERNAME Ihr Nutzername auf dem Rechner ist.

Sollte es beim Zugriff auf die Seite eine Fehlermeldung im Browser geben ("Permission denied"), überprüfen Sie bitte, ob Ihr Homeverzeichnis für alle die x-Berechtigung hat und das Verzeichnis `public_html` für alle r- und x-Berechtigungen hat. Falls nicht, ändern Sie die Berechtigungen mit `chmod a+x ~` und `chmod a+rx ~/public_html`.

Abgabe: URL der Seite


## 9.8 SSL-Stripping
Beschreiben Sie bitte kurz und knapp, was man unter einem __SSL-Stripping__-Angriff versteht.

<div style="border: 1px solid grey;"><br><br><br><br><br><br><br><br><br><br></div>


## 9.9 C/S-Modell vs. P2P
Vergleichen Sie Client/Server-Modell mit dem Peer-to-Peer-Modell und ordnen Sie passend zu:

  * Einer bietet Dienste an, der andere nutzt sie: ....
  * Web-Browsing: ....
  * Bitcoin: ....
  * Alle Parteien sind gleichberechtigt: ....
  * BitTorrent: ....
  * E-Mail: ....

*Antworten:*

  1. Peer-to-Peer
  2. Client/Server


## 9.10 DNS
Zeigen Sie die Schritte auf, die passieren, wenn eine Adresse (z.B. `www.google.com`) in die IP-Adresse aufgelöst wird:

  * Sobald er diese Adresse hat, fragt er dort an, welcher Nameserver für  `google.com` zuständig ist.: ....
  * Wird dort kein Eintrag gefunden, überprüft der Client, ob der Name in seinem lokalen Cache (Zwischenspeicher) vorhanden ist. : ....
  * Sobald er diese Adresse hat, fragt er dort an, ob dieser `www.google.com` kennt bzw. falls nicht, wer den der nächste zuständige Nameserver ist.: ....
  * Verläuft diese Anfrage ergebnislos, wird der DNS-Server konsultiert.: ....
  * Die Datei `hosts` wird durchsucht.: ....
  * Der Nameserver fragt den Root-Server an, wer als Nameserver für `com` zuständig ist: ....

*Antworten:*

  1. Schritt 1
  2. Schritt 2
  3. Schritt 3
  4. Schritt 4
  5. Schritt 5
  6. Schritt 6


## 9.11 HTML vs. CSS
Welche Aufgaben haben HTML, CSS und JavaScript? Ordnen Sie korrekt zu:

  * legt Farben und Hintergründe fest: ....
  * definiert das Layout: ....
  * beschreibt den Inhalt: ....
  * ermöglicht dynamische Inhalte: ....
  * legt Schriftarten fest: ....
  * enthält Texte, Tabellen etc.: ....
  * reagiert auf Aktionen: ....
  * legt die Größe von Schriften fest: ....
  * definiert Tabellen: ....

*Antworten:*

  1. HTML
  2. CSS
  3. JavaScript


## 9.12 Mail-Protokolle
Ordnen Sie die Mail-Protokolle ihren jeweiligen Aufgaben zu:

  * Abholen von Mails vom Server auf den Client: ....
  * Austausch von Mails zwischen Servern (MTAs): ....
  * Verwalten und Lesen von Mails auf dem Server: ....
  * Versenden von Mails vom Client (MUA) zum Server (MTA): ....

*Antworten:*

  1. IMAP
  2. MOP
  3. POP3
  4. SMTP
  5. DHCP
  6. HTTP


## 9.13 DNS
Welchen Zweck hat das Domain Name System (DNS) und wie ist es technisch aufgebaut?

  * [ ] die Auflösung eines Namens erfolgt von hinten nach vorne
  * [ ] es löst IP-Adressen zu Namen auf
  * [ ] die Auflösung einer Adresse erfolgt von vorne nach hinten
  * [ ] es besteht aus Nameservern
  * [ ] es verwendet eine zentrale Datei (`hosts`) in der alle Rechner verzeichnet sind
  * [ ] die Such beginnt bei den Root-Servern
  * [ ] es ist hierarchisch aufgebaut
  * [ ] die Auflösung einer Adresse erfolgt von hinten nach vorne
  * [ ] es ist flach aufgebaut
  * [ ] es löst Namen zu IP-Adressen auf
  * [ ] die Auflösung eines Namens erfolgt von vorne nach hinten

## 9.14 Namensauflösung
Sie finden folgenden Eintrag in der Datei `/etc/hosts` auf Ihrem Rechner (bzw. `C:\Windows\System32\Drivers\etc\hosts`, falls Sie Windows verwenden sollten):

```console
127.0.0.1  localhost
127.0.0.1  www.google.de
```

Was passiert, wenn Sie im Browser die URL `http://www.google.de` eingeben?

  * [ ] es kommt zu einem Absturz des Rechners
  * [ ] der Browser zeigt einen Fehler
  * [ ] es wird die Webseite von Google angezeigt
  * [ ] die DNS-Anfrage dauert deutlich länger
  * [ ] der Browser versucht die Daten vom lokalen Rechner zu beziehen

## 9.15 Elemente einer HTML-Seite
Bitte ordnen Sie den aufgeführten HTML-Tags ihre jeweilige Aufgabe zu:


Geben Sie den ungefähren Aufbau einer HTML-Seite mit den entsprechenden Bereichen (Header, Titel, Meta-Daten, Body, etc.) an. Formulieren Sie Ihre Antwort mit den entsprechenden HTML-Tags.

  * `<h1>`: ....
  * `<meta>`: ....
  * `<script>`: ....
  * `<p>`: ....
  * `<html>`: ....
  * `<h2>`: ....
  * `<title>`: ....
  * `<br>`: ....
  * `<head>`: ....
  * `<a>`: ....
  * `<body>`: ....

*Antworten:*

  1. Wurzelelement; umschließt das gesamte Dokument
  2. Metadaten, z.B. Zeichensatz
  3. Daten zum Dokument, die nicht (direkt) angezeigt werden
  4. Überschrift
  5. Zeilenumbruch
  6. kein HTML-Tag
  7. Umschließt die anzuzeigenden Daten
  8. Absatz
  9. Verweis auf ein anderes Dokument oder eine Stelle im Dokument
  10. Name der Seite, wird im Browserfenster angezeigt
  11. Einbindung von aktiven Inhalten


## 9.16 Hypertext
HTML steht für _HyperText Markup Language_. Welche Aussagen zu _Hypertext_ sind korrekt?

  * [ ] Dokumente enthalten Verweise auf andere Dokumente
  * [ ] Dokumente enthalten andere Dokumente
  * [ ] Dokumente bilden einen Hyperkubus
  * [ ] In HTML ist das `<a>` Tag entscheidend für die Verlinkung der Dokumente
  * [ ] Dokumente enthalten Verweise auf andere Stellen im selben Dokument
  * [ ] In HTML ist das `<link>` Tag entscheidend für die Verlinkung der Dokumente
  * [ ] Dokumente werden miteinander verknüpft
  * [ ] Dokumente enthalten nicht nur Text, sondern auch Bilder und andere Medien
  * [ ] Dokumente bauen eine netzartige Struktur auf

