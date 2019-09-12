# 10. Datenmanagement - Übungen

## 10.1 Datenmodell
Welchen Zweck hat ein Datenmodell?


## 10.2 DBMS vs. Anwendung
Fassen Sie die Aufgaben einer Anwendungssoftware und eines Datenbanksystems zusammen. Warum ist die Trennung sinnvoll, d.h. welche Vorteile bringt sie?


## 10.3 SQL
Worum handelt es sich bei SQL und wofür wird es eingesetzt? Nennen Sie die wichtigsten SQL-Befehle.


## 10.4 Relationen lesen
Beantworten Sie die folgenden Fragen basierend auf der unten dargestellten Datenbankrelation:

  1. Wer ist der Sekretär in der Buchhaltung (Accounting) mit Erfahrungen in der Personalabteilung (Personnel)?
  2. Wer ist der Manager des Vertriebs (Sales)?

_EMPLOYEE_

| EmplId | Name            | Address          | SSN       |
|--------|-----------------|------------------|-----------|
| 25X15  | E. Baker        | 33 Nowhere St.   | 111223333 |
| 34Y70  | H. Clark        | 563 Downtown Ave | 999009999 |
| 23Y34  | G. Smith        | 1555 Circle Dr.  | 111005555 |

_JOB_

| JobId | JobTitle      | SkillCode | Dept       |
|-------|---------------|-----------|------------|
| S25X  | Secretary     | T5        | Personnel  |
| S26Z  | Secretary     | T6        | Accounting |
| F5    | Manager       | FM3       | Sales      |

_ASSIGNMENT_

| EmplId | JobId      | StartDate  | TermDate   |
|--------|------------|------------|------------|
| 23Y34  | S25X       | 1999-03-01 | 30-04-2010 |
| 34Y70  | F5         | 2009-10-01 | NULL       |
| 23Y34  | S26Z       | 2010-05-01 | NULL       |


## 10.5 Relationen auswerten
Beantworten Sie die folgende Frage basierend auf der unten dargestellten Datenbankrelation:

_EMPLOYEE_

| EmplId | Name            | Address          | SSN       |
|--------|-----------------|------------------|-----------|
| 25X15  | E. Baker        | 33 Nowhere St.   | 111223333 |
| 34Y70  | H. Clark        | 563 Downtown Ave | 999009999 |
| 23Y34  | G. Smith        | 1555 Circle Dr.  | 111005555 |

_JOB_

| JobId | JobTitle      | SkillCode | Dept       |
|-------|---------------|-----------|------------|
| S25X  | Secretary     | T5        | Personnel  |
| S26Z  | Secretary     | T6        | Accounting |
| F5    | Manager       | FM3       | Sales      |

_ASSIGNMENT_

| EmplId | JobId      | StartDate  | TermDate   |
|--------|------------|------------|------------|
| 23Y34  | S25X       | 1999-03-01 | 30-04-2010 |
| 34Y70  | F5         | 2009-10-01 | NULL       |
| 23Y34  | S26Z       | 2010-05-01 | NULL       |


Wie kann man die Liste aller Job-Bezeichnungen in der Personalabteilung finden? Übertragen Sie Ihre Antworten in ein SQL-Statements.

  * [ ] `FIND JOB IN Table WHERE Employee ='Personnel'`
  * [ ] `SELECT * FROM JOB WHERE Dept ='Personnel'`
  * [ ] `SELECT * FROM EMPLOYEE WHERE Dept ='Personnel'`
  * [ ] `FIND * FROM JOB WHERE Dept ='Personnel'`
  * [ ] `SELECT JOB FROM Dept WHERE Employee ='Personnel'`

## 10.6 Beziehungen zwischen Tabellen
Wie werden die verschiedenen Beziehungen in einer Datenbank dargestellt? Wie werden 1-n versus n-m-Beziehungen abgebildet?


## 10.7 Transaktion
Was versteht man unter einer Datenbanktransaktion?


## 10.8 Datenbank entwerfen
Entwerfen Sie ein Datenbankschema für die Speicherung von Komponisten, ihren Kompositionen und den Lebensdaten (geboren, gestorben) der Komponisten. Füllen Sie das Schema mit einigen Beispielen.


## 10.9 Datenbank entwerfen
Erweitern Sie die Datenbank aus der vorherigen Aufgabe um die Information, welche Dirigenten Stücke der Komponisten aufgeführt haben. Beachten Sie, dass ein Dirigent mehrere Komponisten aufgeführt haben kann und ein Komponist von mehreren Dirigenten aufgeführt wird. Geben Sie wieder Beispieldaten an.


## 10.10 DBMS vs. Anwendung
Ordnen Sie die Aufgaben einer Anwendungssoftware und eines Datenbanksystems zu.

  * enthält die Daten: ....
  * enthält die Geschäftsregeln: ....
  * erlaubt eine konsistente Sicherung der Daten: ....
  * bietet die Daten anderen Systemen an: ....

*Antworten:*

  1. Anwendungssystem
  2. Datenbanksystem


## 10.11 SQL
Ordnen Sie den Aufgaben die jeweiligen SQL-Befehlen zu:

  * Indices löschen: ....
  * Tabellen löschen: ....
  * Daten in Tabellen einfügen: ....
  * Daten aus Tabellen löschen: ....
  * Daten aus einer Tabelle suchen: ....
  * Indices anlegen: ....
  * Tabellen anlegen: ....

*Antworten:*

  1. `UNTABLE`
  2. `TABLE`
  3. `SELECT`
  4. `CREATE`
  5. `OBLITERATE`
  6. `DELETE`
  7. `INSERT`
  8. `SEARCH`
  9. `INDEX`
  10. `DROP`
  11. `PURGE`
  12. `MAKE`
  13. `ADD`


## 10.12 Relationen lesen
Beantworten Sie die folgende Frage basierend auf der unten dargestellten Datenbankrelation:

_EMPLOYEE_

| EmplId | Name            | Address          | SSN       |
|--------|-----------------|------------------|-----------|
| 25X15  | E. Baker        | 33 Nowhere St.   | 111223333 |
| 34Y70  | H. Clark        | 563 Downtown Ave | 999009999 |
| 23Y34  | G. Smith        | 1555 Circle Dr.  | 111005555 |

_JOB_

| JobId | JobTitle      | SkillCode | Dept       |
|-------|---------------|-----------|------------|
| S25X  | Secretary     | T5        | Personnel  |
| S26Z  | Secretary     | T6        | Accounting |
| F5    | Manager       | FM3       | Sales      |

_ASSIGNMENT_

| EmplId | JobId      | StartDate  | TermDate   |
|--------|------------|------------|------------|
| 23Y34  | S25X       | 1999-03-01 | 30-04-2010 |
| 34Y70  | F5         | 2009-10-01 | NULL       |
| 23Y34  | S26Z       | 2010-05-01 | NULL       |


Wer ist der Manager des Vertriebs (Sales)?

  * [ ] E. Baker
  * [ ] G. Smith
  * [ ] H. Clark

## 10.13 Relationen lesen
Beantworten Sie die folgende Frage basierend auf der unten dargestellten Datenbankrelation:

_EMPLOYEE_

| EmplId | Name            | Address          | SSN       |
|--------|-----------------|------------------|-----------|
| 25X15  | E. Baker        | 33 Nowhere St.   | 111223333 |
| 34Y70  | H. Clark        | 563 Downtown Ave | 999009999 |
| 23Y34  | G. Smith        | 1555 Circle Dr.  | 111005555 |

_JOB_

| JobId | JobTitle      | SkillCode | Dept       |
|-------|---------------|-----------|------------|
| S25X  | Secretary     | T5        | Personnel  |
| S26Z  | Secretary     | T6        | Accounting |
| F5    | Manager       | FM3       | Sales      |

_ASSIGNMENT_

| EmplId | JobId      | StartDate  | TermDate   |
|--------|------------|------------|------------|
| 23Y34  | S25X       | 1999-03-01 | 30-04-2010 |
| 34Y70  | F5         | 2009-10-01 | NULL       |
| 23Y34  | S26Z       | 2010-05-01 | NULL       |


Wer ist der Sekretär in der Buchhaltung (Accounting) mit Erfahrungen in der Personalabteilung (Personnel)?

  * [ ] H. Clark
  * [ ] G. Smith
  * [ ] E. Baker

## 10.14 Relation
In einem Datenbankschema sollen Dirigenten und die von ihnen aufgeführten Stücke gespeichert werden. Ein Stück kann von mehreren Dirigenten aufgeführt werden und ein Dirigent führt unterschiedliche Stücke auf.

Wie würden Sie diese Art von Daten modellieren?

  * [ ] Tabellen `DIRIGENT` und `STUECK`. Der Primärschlüssel von `STUECK` wird zum Fremdschlüssel in `DIRIGENT`
  * [ ] Tabellen `DIRIGENT` und `STUECK` und Verknüpfungstabelle
  * [ ] Tabellen `DIRIGENT` und `STUECK`. Der Primärschlüssel von `DIRIGENT` wird zum Fremdschlüssel in `STUECK`
  * [ ] Tabellen `DIRIGENT` und `STUECK`
  * [ ] Tabelle `DIRIGENT_UND_STUECK`

## 10.15 Beziehungen zwischen Tabellen
Wie werden die verschiedenen Beziehungen in einer Datenbank dargestellt? Wählen Sie die richtigen Aussagen aus:

  * [ ] bei 1-n Beziehungen ist der Primärschlüssel einer Tabelle der Fremdschlüssel einer anderen Tabelle
  * [ ] bei m-n Beziehungen werden die Einträge einer Tabelle an die andere angehängt
  * [ ] bei m-n Beziehungen ist der Primärschlüssel einer Tabelle der Fremdschlüssel einer anderen Tabelle
  * [ ] bei 1-n Beziehungen werden die Einträge einer Tabelle an die andere angehängt
  * [ ] bei m-n Beziehungen gibt es eine weitere Tabelle, die die Primärschlüssel der zu verknüpfenden Einträge enthält
  * [ ] bei 1-n Beziehungen gibt es eine weitere Tabelle, die die Primärschlüssel der zu verknüpfenden Einträge enthält

## 10.16 Transaktion
Was versteht man unter einer Datenbanktransaktion?

  * [ ] Folge von Schritten, die den Datenbestand nach fehlerfreier und vollständiger Ausführung in einem konsistenten Zustand hinterlassen
  * [ ] Folge von Schritten, die den Datenbestand an eine andere Datenbank übertragen und ununterbrechbar ablaufen
  * [ ] Darstellung eines Buchhaltungsvorgangs in einer Datenbank, wobei immer eine Soll- und Habenbuchung gleichzeitig erfolgen

## 10.17 Datenbank verstehen
Gegeben sei das folgende Datenbankschema.

_KOMPONIST_

| ID | Nachname  | Vorname    | geboren    | gestorben  |
|----|-----------|------------|------------|------------|
|  1 | Bach      | Johann     | 1685-03-31 | 1750-07-28 |
|  2 | Cage      | John       | 1912-09-05 | 1992-08-12 |
|  3 | Riehm     | Rolf       | 1937-06-15 | NULL       |

_WERK_

| ID | Komponist | Titel                |
|----|-----------|----------------------|
|  1 |         1 | Magnificat           |
|  2 |         1 | Triosonaten          |
|  3 |         1 | Englische Suiten     |
|  4 |         2 | Imaginary Landscapes |
|  5 |         2 | 4:33                 |
|  6 |         3 | Abrazzo-Oper         |
|  7 |         3 | Gewidment            |


Welche Stücke sind von John Cage?

  * [ ] Magnificat
  * [ ] Abrazzo-Oper
  * [ ] Imaginary Landscapes
  * [ ] Englische Suiten
  * [ ] Gewidment
  * [ ] Triosonaten
  * [ ] 4:33

