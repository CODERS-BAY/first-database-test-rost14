# DB-Test
## Aufgabe 1
Stelle Entitäten mittels Chen-Notation und Min,Max Notation dar.<br>
Wähle ein sinnvolles Beispiel!

![](Aufgabe1.png)

## Aufgabe 2
Kann eine Beziehung Attribute haben?

Ja

Wenn ja, wie stelle ich es im ERD dar?

Wird als assoziative Tabelle dargestellt.
## Aufgabe 3
Welche Codd'schen Anforderungen gibt es (Nenne mindestens 5)

Integration<br>
Operationen<br>
Katalog <br>
Benutzeransichten<br>
Integrität<br>
Datensicherung<br>
Transaktionen<br>
Zugriffskontrolle<br>
Synchronisation

  
## Aufgabe 4
Nenne den Unterschied zwischen Konzeptuellen und Logischem Schema

Konzeptuelles Schema: Grafische und textuelle Notationen

Logisches Schema: Tabellarische Darstellung

## Aufgabe 5
Welche 3 Bestandteile gibt es im Entity Relationship Model

Entity = Objekt <br>
Relation = Beziehung zwischen den Objekten<br>
Attribute = Eigenschaften von einem Objekt oder Beziehung<br>
## Aufgabe 6
Welche Datentypen gibt es in MySQL? (Nenne mindestens 5)

Integer, double, varchar, char, Blob (Binary large object) date, timestamp
## Aufgabe 7
Welche Arten von Schlüsseln gibt es und welche Eigenschaften besitzen diese?

Primärschlüssel: dient zur eindeutigen Identifikation eines Objekts

Fremdschlüssel: ist ein Schlüssel in einer Tabelle um auf andere Tabellen zu verweisen und diese zu verbinden. ein Fremdschlüssel muss immer ein Primärschlüssel in jener Tabelle sein auf die er verweist.
## Aufgabe 8
Welche Arten von Beziehungen gibt es? Zeichne für jede ein Beispiel auf


unär: Eine Entität hat eine Beziehung mit sich selbst


binär: Beziehung zwischen zwei Entitäten


ternär: Beziehung zwischen drei oder mehr Entitäten


## Aufgabe 9
Was bedeutet der Begriff Kardinalität und welche Kardinalitäten gibt es?

Kardinalität = Verhältnisse der Beziehungen

1 : 1

1 : n

m : n

## Aufgabe 10
Was bedeutet der Begriff Datenintegrität und worin unterscheidet sich Integrität und referentielle Integrität?

Datenintegrität = Richtigkeit der Daten

Referentielle Integrität =  Richtigkeit der Beziehungen

## Aufgabe 11
Erkläre die 3 Normalformen

1.Normalform:
Beziehungsschema wird in seine atomaren Bestandteile zerlegt.

2.Normalform:
Das Beziehungsschema erfüllt die 1.Normalform und alle Nichtschlüsselattribute sind vom Primärschlüssel
voll funktional abhängig.

3.Normalform:
Das Beziehungsschema erfüllt die 2.Normalform und kein Nichtschlüsselattribut ist vom Primärschlüssel
transitiv abhängig und kein Nichtschlüsselattribut hängt von einem Nichtschlüsselattribut ab. 

## Aufgabe 12
Erkläre den Unterschied zwischen starken und Schwachen Entitäten und erstelle ein Beispiel.


Starke Entität: Kann für sich alleine exestieren und ist nich von anderen abhängig.


Schwache Entität: Kann nur in Verbindung mit einer anderen Entität existieren.


Beispiel: Ein Haus kann ohne einen Raum existieren, aber ein Raum nicht ohne eine Haus.

## Aufgabe 13
Welche Grundregeln gibt es im Relationenmodell? (Nenne mindestens 4)

Jede Entität braucht eine eindeutige Bezeichnung (Primärschlüssel oder ein zusammengesetzter Schlüssel)


Alle Entitäten müssen über Beziehungen verbunden sein


Keine Daten sollen doppelt vorhanden sein (Redundanz vermeiden)


Keine n:m Beziehungen (auflösen mit Kreuztabelle bzw. Beziehung als Entität) 
## Aufgabe 14
Wie löst man eine M:N Beziehung auf? Erstelle ein Beispiel

Die n:m-Beziehung wird aufgelöst und man erhält eine weitere Datenbanktabelle die 1:n-Beziehungen realisiert. 


## Aufgabe 15
Ein Handelsbetrieb verkauft ein Sortiment von Artikeln, die er von verschiedenen Herstellern bezieht. Der Handelsbetrieb hat einen bestimmten Kundenkreis, der regelmäßig Bestellungen aufgibt. Eine Bestellung kann mehrere Artikel umfassen. Ein Artikel kann von mehreren Lieferanten bezogen werden und ein Lieferant liefert natürlich meist mehr als einen Artikel. Erstelle ein ERD und ein Relationenmodell, welches der 3. Normalform entspricht.
## Aufgabe 16
Welche Anomalien kennst du und was beschreiben sie?


Insert: Wenn falsche oder redundante Daten eingetragen werden.


Update: Wenn beim hinzufügen oder aktualisieren mehrere Daten oder andere Daten verfälscht werden.


Delete: Wenn beim löschen von Daten andere Daten ebenfalls gelöscht werden.


## Aufgabe 17
Modellieren Sie den angeführten Realitätsausschnitt einer Fluggesellschaft mit Hilfe eines Entity Relationship- Diagramms. Treffen Sie, falls notwendig, sinnvolle Annahmen und dokumentieren Sie diese nachvollziehbar in Ihrer Lösung. Der zu betrachtende Realitätsausschnitt der Fluggesellschaft umfasst folgenden
Sachverhalt:
Flughäfen haben ein Kürzel (= Schlüssel) und gehören zu einer Stadt (z.B. „FRA“ für Frankfurt, „FCO“ für Roma Fiumicino).
Flüge haben eine Flugnummer (z.B. „LH 306“), führen von einem Flughafen zu einem anderen, mit jeweils einer festen Abflugs- und Ankunftszeit (z.B. ab Frankfurt um 07:30 nach Roma Fiumicino mit Ankunft um 09:15).
Jeder Flugzeugtyp hat einen Namen (z.B. „747-400“) und eine Sitzanzahl (z.B. 430 Sitze).
Piloten haben einen Namen (z.B. „Meier“), ein Geburtsdatum (z.B. „1.1.1960“) und eine Berechtigung, bestimmte Flugzeugtypen zu fliegen (z.B. „747-400“ und „A310“).
Jedes einzelne Flugzeug ist von einem bestimmten Flugzeugtyp (z.B. „747-400“) und hat einen Namen (z.B. „Mozart“).
Bei einem Flug-Einsatz wird ein Flug (z.B. „LH 306“) an einem bestimmten Datum (z.B. „6.2.2011“) von einem bestimmten Piloten (z.B. „Meier“) mit einem bestimmten Flugzeug (z.B. „Mozart“) geflogen.
Bilden Sie das konzeptuelle Schema in ein relationales Schema ab. Das relationale Schema soll der 3. Normalform genügen
