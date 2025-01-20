# Einführung

Notizen
Daten: Daten können in verschiedenen formen vorhanden, z. B. in Dokumenten,
Audios, Videos (HTML hat auch Daten in sich), die müssen zu uns gelangen.

Es sind gespeicherte Informationen im Internet.
Frage: Wie können Daten gespeichert sein und was hat das mit dem ASCII-Code zu tun?
Wo sind die Daten gespeichert? - Auf ganz kleinen Karten, z. B. SD-Karten, Festplatten.
Dieser hat ganz viele Speicherzellen. Einige Zellen sind eingeschaltet, einige nicht.
Z. B. 1, 0, 1, 0, 1, 0, 0, 1,  Man kann nur sagen, ob diese Speicherzellen aktiviert oder deaktiviert sind.
Wie kann man Daten von einem Gerät zum anderen übertragen? - Man bracuht eine Verbindung zwischen zwei Geräten.

Dann kann man sagen, - Der Empfänger erkennt, wenn es Strom oder kein Strom kriegt. Diese Signale können zu 0 und 1 interpretiert werden.
Das ist ähnlich wie Morse-Code. Bei 1000 Bits pro Sekunde, wird bei jeder ein Tausendtsel Sekunde geschaut, ob es Strom gibt oder nicht.
Das hat mit dem komplizierten Binärsystem etwas zu tun. Der Computer kann nur Bits etwas speichern.
Von 8 Bits kommt man auf eine Zahl und kann dann auf ACII-Code nachsehen - z. B. 0110 - 65 - "A"
Direkt muss man zuerst mit 0 und 1 schreiben. - aber wie kommt man überhaupt von 0 und 1 auf die Zahl für den ASCII?
shift + recht von ? =

```JSON
{
    "Vorname": "Peter",
    "Nachname": "Muster"
}

```

um den Code praktisch zu beschreiben, ist ähnlich wie Kommentare.
Z. B. Im Schulnetz werden Daten von uns gespeichert und von irgendwoher gelesen - Modellierung von Daten
JSON ist eine Beschreibungssprache, keine wirkliche Programmierssprache.
Aufgabe: Ein eigenes Objekt modellieren: Buch.
```JSON
{
    "Titel": "Farm der Tiere"
    "Autor": "George Orwell"
    "Erscheinungsjahr":"1945"
    "Anzahl Seiten": "90 - 130 Seiten"
 }

```
Reduntant wären Informationen, wenn man z. B. das Alter und das Geburtsdatum des Autors schreibt. Das eine kann man vom anderen ableiten.

Sind reduntante Informationen schlimm? - Manchmal praktisch, manchmal nicht. Meisten möchte man Redundanz jedoch vermeiden (überflüssig).

Es gibt auch praktische Redundanz: Bei ganz kritischen Daten, z. B. das Gesamtvermögen auf einer Bank, kann das Geld einmal in Franken und einmal in Rappen geschickt werden, um zu überprüfen, ob es eine Korruption gibt. Das macht man bei ganz wichtigen Daten. Beim Modellieren ist die Redundanz jedoch sehr schlecht.
Datenansicht und Datenspeicherung - bei der Datenspeicherung ist Redundanz unerwünscht.
Mögliche Prüfungsfrage: Was ist Redundanz und wieso ist das schlecht?

Vergleich: Wenn man zum Beschreiben eines Wortes zwei Synonyme verwendet. Es ist schlicht unnötig.

Wie unterscheiden sich Datenansicht und Datenspeicherung?

Was sind berechnete Attribute und was haben diese mit Redundanz zu tun?

Geben Sie ein Beispiel mit einem Objekt mit/und ohne Redundanz. Welche Attribute sind reduntant? Würde es trotzdem Sinn machen, dieses Objekt so zu verwenden? Wenn nicht, geben Sie ein Beispiel an, das Sinn macht.

Erklären Sie, wie Daten gespeichert werden und wie diese über das Internet getragen werden (oder von Gerät zu Gerät)
