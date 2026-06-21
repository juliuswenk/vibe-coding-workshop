---
layout: default
title: Mein erstes Projekt
---

# Mein erstes Projekt: Poster-Generator

## Was diese Seite erklärt

In diesem Abschnitt bauen wir gemeinsam einen kleinen interaktiven `Poster-Generator`.

Ein `Poster-Generator` ist eine einfache Website, auf der du ein digitales Poster verändern kannst: Farben wechseln, Layouts ausprobieren, Formen zufällig anordnen und Texte anpassen.

Wir bauen keine perfekte App. Wir bauen eine erste funktionierende Version, damit du den Workflow mit einem `Coding Agent` verstehst:

1. Ziel beschreiben
2. Grenzen setzen
3. Plan prüfen
4. kleine Änderung erlauben
5. Ergebnis testen
6. Feedback geben

## Warum das für Vibe Coding wichtig ist

Der Poster-Generator ist klein genug für den Einstieg, aber groß genug, um echtes Vibe Coding zu üben.

Du lernst dabei, wie du ein Projekt in kleinere Teile zerlegst. Das ist wichtig, weil ein `Coding Agent` bessere Ergebnisse liefert, wenn du ihm nicht alles auf einmal gibst.

Du übst außerdem, klare Grenzen zu setzen:

- keine externen Frameworks
- keine Datenbank
- kein Login
- nur `HTML`, `CSS` und `JavaScript`
- erst planen, dann Dateien ändern

So bleibst du in Kontrolle. Der Agent schreibt Code, aber du entscheidest, was gebaut wird und wann der nächste Schritt kommt.

---

## Vorbereitung

Bevor wir starten, solltest du ein eigenes `Repository` auf GitHub angelegt haben.

Ein `Repository` ist der Projektordner auf GitHub. Dort liegen später deine Dateien, zum Beispiel `index.html`, `style.css` und `script.js`.

Öffne dein Repository in `Zed` und starte dort deinen `Coding Agent`.

Wenn du noch nicht so weit bist, gehe zuerst zurück zur GitHub-Anleitung.

## Ziel des Projekts

Am Ende soll eine kleine Website entstehen, die du im Browser öffnen kannst.

| Bestandteil | Mindestziel |
| --- | --- |
| Posterfläche | Eine große sichtbare Fläche im Browser |
| Titeltext | Ein Text, der auf dem Poster steht |
| Formen | Abstrakte grafische Elemente |
| Farbpaletten | Mindestens drei auswählbare Varianten |
| Layouts | Mindestens drei unterschiedliche Anordnungen |
| `Randomize` | Ein Button für neue zufällige Kompositionen |

Ein Screenshot reicht als Ergebnis. Wir brauchen keine Exportfunktion.

---

## Gemeinsamer Bauprozess

### Schritt 1: Einen Plan verlangen

Jetzt beschreiben wir das Projekt, aber wir lassen noch keine Dateien ändern.

Kopiere diesen Prompt:

```text
Ich möchte einen interaktiven Poster-Generator bauen.

Nutze nur HTML, CSS und JavaScript.
Nutze keine externen Frameworks.
Baue keine Datenbank, kein Login und keine Exportfunktion.

Die Website soll enthalten:
- eine große Posterfläche
- einen Titeltext
- abstrakte grafische Formen
- Buttons für mindestens drei Farbpaletten
- Buttons für mindestens drei Layout-Varianten
- einen Randomize-Button

Erstelle zuerst einen kurzen Plan in 3 bis 5 Schritten.
Nenne genau, welche Dateien du erstellen oder ändern würdest.
Ändere noch keine Dateien.
```

Lies den Plan. Er sollte ungefähr so aussehen:

- `index.html` für die Struktur
- `style.css` für Gestaltung und Posterfläche
- `script.js` für Buttons und Zufall

Wenn der Agent mehr bauen will, zum Beispiel ein Framework, eine Datenbank oder viele neue Ordner, stoppe ihn:

```text
Bitte halte es einfacher.
Nutze nur index.html, style.css und script.js.
Keine Frameworks und keine zusätzlichen Tools.
```

### Schritt 2: Erste Version bauen lassen

Wenn der Plan sinnvoll klingt, erlaubst du die erste Änderung.

Kopiere diesen Prompt:

```text
Der Plan ist okay.

Erstelle jetzt die erste einfache Version.

Wichtig:
- Nutze nur HTML, CSS und JavaScript.
- Halte den Code einfach verständlich.
- Erstelle nur die Dateien, die du im Plan genannt hast.
- Baue zuerst nur die Grundversion mit Posterfläche, Titel, Formen und Buttons.

Erkläre danach kurz:
1. Welche Dateien du erstellt oder geändert hast.
2. Wie ich die Seite im Browser öffnen kann.
3. Was noch nicht eingebaut ist.
```

### Schritt 3: Website im Browser öffnen

Jetzt öffnest du die Website, damit du das Ergebnis sehen kannst.

Wenn der Agent eine Datei `index.html` erstellt hat:

1. Suche die Datei `index.html` links im Dateibaum von `Zed`.
2. Klicke mit der rechten Maustaste auf `index.html`.
3. Wähle eine Option wie `Reveal in Finder`, `Im Finder anzeigen` oder `Im Explorer anzeigen`.
4. Öffne die Datei dann mit einem Doppelklick im Browser.

Wenn dein Browser die Datei öffnet, siehst du oben in der Adresszeile meistens einen Pfad, der mit `file://` beginnt. Das ist okay. Es bedeutet nur, dass du die Datei direkt von deinem Computer geöffnet hast.

Falls dein Agent einen lokalen Server gestartet hat, gibt er dir wahrscheinlich eine Adresse wie diese:

```text
http://localhost:3000
```

Kopiere diese Adresse in deinen Browser.

`localhost` bedeutet: Die Website läuft gerade nur auf deinem eigenen Computer.

Prüfe:

1. Siehst du eine Posterfläche?
2. Sind Buttons sichtbar?
3. Passiert etwas, wenn du Buttons klickst?
4. Gibt es Fehlermeldungen?
5. Hat der Agent ungefragt mehr gebaut als nötig?

### Schritt 4: Feedback geben

Jetzt kommt der wichtigste Teil: Du gibst konkretes Feedback.

Schlecht:

```text
Mach es schöner.
```

Besser:

```text
Das Poster wirkt noch zu leer.
Bitte füge mehr abstrakte Formen hinzu.
Ändere nur CSS und JavaScript.
Die Buttons und die bestehende Struktur sollen bleiben.
```

Oder:

```text
Die Layouts sehen noch zu ähnlich aus.
Bitte mache drei klar unterschiedliche Layout-Varianten:
1. ein ruhiges Layout mit viel Leerraum
2. ein dichtes Layout mit vielen Formen
3. ein diagonales Layout mit starker Bewegung

Ändere nur, was dafür nötig ist.
```

Nach jeder Änderung prüfst du wieder im Browser.

### Schritt 5: Randomize verbessern

Wenn die Grundversion funktioniert, verbessern wir den `Randomize`-Button.

Kopiere diesen Prompt:

```text
Verbessere den Randomize-Button.

Wenn man klickt, sollen sich ändern:
- Positionen der Formen
- Größen der Formen
- Farben innerhalb der gewählten Palette
- Rotation der Formen

Der Code soll einfach verständlich bleiben.
Erkläre danach, welche Funktion für die zufällige Komposition verantwortlich ist.
```

Prüfe danach:

1. Verändert sich das Poster sichtbar?
2. Bleibt der Text lesbar?
3. Funktionieren die anderen Buttons noch?

### Schritt 6: Optional Bewegung hinzufügen

Wenn noch Zeit ist, kannst du eine kleine Animation ergänzen.

Kopiere diesen Prompt:

```text
Füge eine dezente Animation hinzu.

Die Formen dürfen sich langsam bewegen oder leicht pulsieren.
Es soll einen Button geben, mit dem man Bewegung ein- und ausschalten kann.

Die Animation soll nicht vom Text ablenken.
Halte die Lösung einfach.
```

Wenn die Animation unruhig wirkt, gib direkt Feedback:

```text
Die Animation ist zu stark.
Bitte mache sie langsamer und reduziere die Bewegung.
Der Text soll im Mittelpunkt bleiben.
```

### Schritt 7: Review machen lassen

Zum Schluss lässt du den Agenten das Projekt prüfen, ohne direkt etwas zu ändern.

Kopiere diesen Prompt:

```text
Bitte reviewe den Poster-Generator.

Ändere keine Dateien.

Prüfe:
- Sind die Controls verständlich?
- Sind die Layouts wirklich unterschiedlich?
- Hat der Code unnötige Komplexität?

Schlage nur einen nächsten Schritt vor.
```

Wichtig: Der Agent soll hier nur analysieren. Du entscheidest danach, ob noch etwas geändert wird.

---

## Gute Abschlussfrage

Beende die Arbeit nicht sofort, sobald etwas funktioniert.

Lass dir den Stand zusammenfassen:

```text
Fasse zusammen:
1. Was wurde gebaut?
2. Welche Dateien wurden geändert?
3. Wie teste ich das Projekt?
4. Was wäre der sinnvollste nächste Schritt?
5. Gibt es bekannte Probleme oder Risiken?
```

Diese Zusammenfassung hilft dir, später wieder einzusteigen.

## Was du jetzt gelernt hast

Du hast ein erstes kleines Browser-Projekt mit einem Coding Agent gebaut.

Dabei hast du geübt:

- ein Ziel verständlich zu beschreiben
- technische Grenzen zu setzen
- zuerst einen Plan einzufordern
- Änderungen in kleinen Schritten zu erlauben
- Ergebnisse im Browser zu prüfen
- Feedback konkret zu formulieren
- den Agenten am Ende reviewen zu lassen

Das ist der wichtigste Workflow für dein eigenes Projekt: klein starten, prüfen, verbessern und die Kontrolle behalten.
