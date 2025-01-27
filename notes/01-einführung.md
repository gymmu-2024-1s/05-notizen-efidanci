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
    "Titel": "Farm der Tiere",
    "Autor": "George Orwell",
    "Erscheinungsjahr":"1945",
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

Warum ist Redundanz unnötig: -unübersichtlich (Überlastung bei zu vielen Daten).
Also Speicherplatz (aber gilt nicht wirklich als Argument, weil sehr billig). ZB. bei Angaben von cm und m muss angepasst werden.

Prüfungsrelevant: Was ist Redundanz, warum ist das gut, warum schlecht?


Was sind Objekte?
Dinge, die im Code vorkommen, die verschiedene Eigenschaften zusammenpacken.
ZB. Objekt: Ball, Information, Radius etc. Mehrere Objekte innerhalb einer Simulation ist möglich. Prüfungsfrage: Erster Ball vorgegeben in einem Code, zweiter Ball horizontal, andere Farbe fliegen lassen. (Objekt hinzufügen, ändern). Ball 3 mit sehr grossem Radius, horizontal fliegen lassen, Farbe dunkelgrün.

Objekte effektiv zusammenfassen, zB. Wohnort, statt Strasse, Plz, Stadt etc. Und falls Informationen verändert werden sollen (ZB. Adresse)
kann das mühsam bzw. ineffektiv sein. Wann ist Verschachtlung gut und wann nicht?
Praktisch, weil, wenn man weiss, dass es sich um die Adresse handelt (Informationen über die Adresse im Objekt drin; Objekt in Objekt), deshalb kann man das einfach überspringen, wenn man möchte. Es ist also übersichtlicher.
Schlecht: Offiziele Sachen, beidem alles sehr gut sichtbar sein soll.

Gutes Beispiel: Medizinische Hintergrundgeschichte
Schlechtes Beispiel: Name als Abschnitt
Einfache Prüfungsfrage: Alternative Darstellung von Objekten angeben, erklären warum es besser ist, Beispiel: Adresse

Listen: Einträge werden mit Komma eingetragen, Resultatsliste ohne Eingabe am Anfang
Vor den einzelnen Objekten brauchen wir keine Schlüssel; das ist der Vorteil bei Listen. (Zusatzfrage)

Beim Programmieren unterscheiden wir Objekt und Klasse. Ein OBjekt ist ein Ding, eine Repräsentation im Code. Ein Objekt ist eine Instanz einer Klasse.Das Objekt lebt im Code mit spezifischen Eigenschaften. Klassen sind Baupläne für Objekte. Vorname, Nachname etc. sind Klassen. Es bestimmt, was für Informationen das Objekt erhalten soll. Instanz einer Klasse richtig einordnen.
Die Klassen bestimmen, welche Informationen/Eigenschaften in einem Objekt vorkommen sollen und die Objekte erhalten dann die genaue Information, die verlangt wird. ZB. Spielfigur: Beim Prorammieren gibt es Klassen, dem werden dann Werte (Objekte) zugewiesen.

Aufgabe: Schema erstellen

```js
class Saeugetiere{
    hat_Fell
    sexuelle_Fortpflanzung
    vier_Gliedermassen
    besitzen_Milchdrüsen

}

class Reptilien{
      hat_Schuppen
    }

```


Vererbung: Beispiel: Haustier mit Vererbung. Wenn Fisch "Haustiere" erweitert (extends) werden alle Klassen vom "Haustiere" übernommen + mehr, falls bei "Fisch" angegeben. Also: Alles aus der Basisklasse + bei Fisch
Vererbung: Man erbt von einer anderen "Klasse". Er übernimmt also alle Iegenschaften.
