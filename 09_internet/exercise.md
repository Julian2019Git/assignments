# 9. WWW und Internet - Übungen

## 9.1 C/S-Modell vs. P2P
Vergleichen Sie Client/Server-Modell mit dem Peer-to-Peer-Modell. Geben Sie Beispiele für die beiden Modelle.


## 9.2 DNS
Wie funktioniert die Auflösung einer Adresse (z.B. `www.google.com`) in die IP-Adresse? Wo kommt das DNS ins Spiel?


## 9.3 Mail-Protokolle
Wieso gibt es für den Umgang mit E-Mails drei Protokoll (SMTP, POP3, IMAP)?


## 9.4 HTTPS
Was ist der Unterschied zwischen dem Zugriff auf die URL `http://stargazer.universe.org` und `https://stargazer.universe.org`?

  * [ ] Der Zugriff auf den Server mit der `https`-URL erfolgt verschlüsselt
  * [ ] Der Zugriff auf den Server mit der `http`-URL erfolgt verschlüsselt
  * [ ] Der Zugriff auf den Server mit der `http`-URL erfolgt über einen Proxy
  * [ ] Der Zugriff auf den Server mit der `https`-URL erfolgt über einen Proxy
  * [ ] Es sind keine gültigen URLs

## 9.5 HTTPS
Welche Aussagen über HTTPS sind korrekt?

  * [ ] die Kommunikation erfolgt verschlüsselt
  * [ ] es basiert auf SSH
  * [ ] es verwendet Zertifikate
  * [ ] die Speicherung der Daten erfolgt verschlüsselt
  * [ ] der Browser kann sich gegenüber dem Server identifizieren
  * [ ] es verschlüsselt die Daten asymmetrisch
  * [ ] es verwendet PGP-Keys
  * [ ] es basiert auf SSL/TLS
  * [ ] der Server identifiziert sich gegenüber dem Browser

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

  * Alle Parteien sind gleichberechtigt: ....
  * BitTorrent: ....
  * E-Mail: ....
  * Einer bietet Dienste an, der andere nutzt sie: ....
  * Web-Browsing: ....
  * Bitcoin: ....

*Antworten:*

  1. Client/Server
  2. Peer-to-Peer


## 9.10 DNS
Zeigen Sie die Schritte auf, die passieren, wenn eine Adresse (z.B. `www.google.com`) in die IP-Adresse aufgelöst wird:

  * Sobald er diese Adresse hat, fragt er dort an, ob dieser `www.google.com` kennt bzw. falls nicht, wer den der nächste zuständige Nameserver ist.: ....
  * Der Nameserver fragt den Root-Server an, wer als Nameserver für `com` zuständig ist: ....
  * Die Datei `hosts` wird durchsucht.: ....
  * Verläuft diese Anfrage ergebnislos, wird der DNS-Server konsultiert.: ....
  * Sobald er diese Adresse hat, fragt er dort an, welcher Nameserver für  `google.com` zuständig ist.: ....
  * Wird dort kein Eintrag gefunden, überprüft der Client, ob der Name in seinem lokalen Cache (Zwischenspeicher) vorhanden ist. : ....

*Antworten:*

  1. Schritt 1
  2. Schritt 2
  3. Schritt 3
  4. Schritt 4
  5. Schritt 5
  6. Schritt 6


## 9.11 HTML vs. CSS
Welche Aufgaben haben HTML, CSS und JavaScript? Ordnen Sie korrekt zu:

  * enthält Texte, Tabellen etc.: ....
  * ermöglicht dynamische Inhalte: ....
  * legt Schriftarten fest: ....
  * definiert Tabellen: ....
  * beschreibt den Inhalt: ....
  * reagiert auf Aktionen: ....
  * definiert das Layout: ....
  * legt die Größe von Schriften fest: ....
  * legt Farben und Hintergründe fest: ....

*Antworten:*

  1. HTML
  2. CSS
  3. JavaScript


## 9.12 Mail-Protokolle
Ordnen Sie die Mail-Protokolle ihren jeweiligen Aufgaben zu:

  * Austausch von Mails zwischen Servern (MTAs): ....
  * Versenden von Mails vom Client (MUA) zum Server (MTA): ....
  * Abholen von Mails vom Server auf den Client: ....
  * Verwalten und Lesen von Mails auf dem Server: ....

*Antworten:*

  1. IMAP
  2. DHCP
  3. MOP
  4. SMTP
  5. HTTP
  6. POP3


## 9.13 DNS
Welchen Zweck hat das Domain Name System (DNS) und wie ist es technisch aufgebaut?

  * [ ] die Such beginnt bei den Root-Servern
  * [ ] es verwendet eine zentrale Datei (`hosts`) in der alle Rechner verzeichnet sind
  * [ ] die Auflösung einer Adresse erfolgt von vorne nach hinten
  * [ ] die Auflösung einer Adresse erfolgt von hinten nach vorne
  * [ ] es besteht aus Nameservern
  * [ ] es ist hierarchisch aufgebaut
  * [ ] die Auflösung eines Namens erfolgt von hinten nach vorne
  * [ ] es löst Namen zu IP-Adressen auf
  * [ ] die Auflösung eines Namens erfolgt von vorne nach hinten
  * [ ] es löst IP-Adressen zu Namen auf
  * [ ] es ist flach aufgebaut

## 9.14 Namensauflösung
Sie finden folgenden Eintrag in der Datei `/etc/hosts` auf Ihrem Rechner (bzw. `C:\Windows\System32\Drivers\etc\hosts`, falls Sie Windows verwenden sollten):

```console
127.0.0.1  localhost
127.0.0.1  www.google.de
```

Was passiert, wenn Sie im Browser die URL `http://www.google.de` eingeben?

  * [ ] die DNS-Anfrage dauert deutlich länger
  * [ ] es kommt zu einem Absturz des Rechners
  * [ ] es wird die Webseite von Google angezeigt
  * [ ] der Browser versucht die Daten vom lokalen Rechner zu beziehen
  * [ ] der Browser zeigt einen Fehler

## 9.15 Elemente einer HTML-Seite
Bitte ordnen Sie den aufgeführten HTML-Tags ihre jeweilige Aufgabe zu:


Geben Sie den ungefähren Aufbau einer HTML-Seite mit den entsprechenden Bereichen (Header, Titel, Meta-Daten, Body, etc.) an. Formulieren Sie Ihre Antwort mit den entsprechenden HTML-Tags.

  * `<a>`: ....
  * `<head>`: ....
  * `<meta>`: ....
  * `<br>`: ....
  * `<script>`: ....
  * `<body>`: ....
  * `<h2>`: ....
  * `<p>`: ....
  * `<title>`: ....
  * `<h1>`: ....
  * `<html>`: ....

*Antworten:*

  1. Metadaten, z.B. Zeichensatz
  2. kein HTML-Tag
  3. Einbindung von aktiven Inhalten
  4. Überschrift
  5. Absatz
  6. Wurzelelement; umschließt das gesamte Dokument
  7. Verweis auf ein anderes Dokument oder eine Stelle im Dokument
  8. Name der Seite, wird im Browserfenster angezeigt
  9. Zeilenumbruch
  10. Daten zum Dokument, die nicht (direkt) angezeigt werden
  11. Umschließt die anzuzeigenden Daten


## 9.16 Hypertext
HTML steht für _HyperText Markup Language_. Welche Aussagen zu _Hypertext_ sind korrekt?

  * [ ] In HTML ist das `<link>` Tag entscheidend für die Verlinkung der Dokumente
  * [ ] Dokumente enthalten Verweise auf andere Stellen im selben Dokument
  * [ ] Dokumente enthalten andere Dokumente
  * [ ] Dokumente enthalten Verweise auf andere Dokumente
  * [ ] Dokumente bauen eine netzartige Struktur auf
  * [ ] Dokumente bilden einen Hyperkubus
  * [ ] Dokumente werden miteinander verknüpft
  * [ ] Dokumente enthalten nicht nur Text, sondern auch Bilder und andere Medien
  * [ ] In HTML ist das `<a>` Tag entscheidend für die Verlinkung der Dokumente

