---
layout: default
title: OpenCode Tutorial
---

# OpenCode Tutorial

In diesem Tutorial lernst du, wie du `OpenCode` in `Zed` nutzt.

OpenCode ist ein `Coding Agent`: Du gibst ihm Aufgaben, Fragen und Feedback. Der Agent kann dein Projekt lesen, Änderungen vorschlagen und beim Bauen deines Projekts helfen.

## Was diese Seite erklärt

Diese Seite erklärt:

- was OpenCode ist
- wie OpenCode in Zed eingebunden wird
- was das Agent Panel ist
- was Threads sind
- wie du einen OpenCode-Thread startest
- welche Optionen wichtig sind
- wie du ein Modell auswählst
- wie du dem Agenten guten Kontext gibst
- wie du Änderungen prüfst
- wann du einen neuen Thread starten solltest

## Warum das für Vibe Coding wichtig ist

Vibe Coding funktioniert nur gut, wenn du den Agenten gezielt führst.

OpenCode kann dir helfen, schneller von einer Idee zu einer sichtbaren Version zu kommen. Aber der Agent braucht klare Aufgaben, Kontext und Grenzen.

Wenn du OpenCode in Zed nutzt, arbeitest du direkt im Projekt. Das bedeutet:

- Der Agent kann deine Dateien sehen.
- Du kannst Änderungen direkt prüfen.
- Du kannst Git nutzen, um gute Zwischenstände zu speichern.
- Du kannst in kleinen Schritten weiterarbeiten.

## Was ist OpenCode?

`OpenCode` ist ein Coding Agent.

Ein Coding Agent ist mehr als ein Chatbot. Er kann mit deinem Projekt arbeiten:

- Dateien lesen
- Code erklären
- Änderungen planen
- Dateien ändern
- Fehlermeldungen analysieren
- Befehle vorschlagen oder ausführen, wenn du es erlaubst

Wichtig: OpenCode ist ein Werkzeug. Es ersetzt nicht dein eigenes Denken.

Du entscheidest:

- Was soll gebaut werden?
- Welche Änderung ist erlaubt?
- Wann ist ein Ergebnis gut genug?
- Was wird gespeichert?

## OpenCode in Zed installieren

Zed kann externe Agents über die `ACP Registry` installieren.

`ACP` steht für `Agent Client Protocol`. Für dich heißt das einfach: Zed kann OpenCode als externen Agenten einbinden.

So installierst du OpenCode in Zed:

1. Öffne `Zed`.
2. Öffne die Command Palette.
   - macOS: `Cmd + Shift + P`
   - Windows: `Ctrl + Shift + P`
3. Suche nach:

```text
zed: acp registry
```

4. Öffne die ACP Registry.
5. Suche nach `OpenCode`.
6. Installiere OpenCode.
7. Starte Zed neu, falls Zed dich dazu auffordert.

Was bringt das?

Nach der Installation kann OpenCode direkt im Agent Panel von Zed genutzt werden. Du musst dann nicht ständig zwischen Editor und externem Terminal wechseln.

## Agent Panel öffnen

Das `Agent Panel` ist der Bereich in Zed, in dem du mit einem Agenten arbeitest.

Du öffnest es über:

- das ✨-Symbol in Zed
- oder die Command Palette mit:

```text
agent: new thread
```

Was bringt das?

Das Agent Panel hält deine Unterhaltung mit dem Agenten direkt neben deinem Projekt. Du kannst Fragen stellen und gleichzeitig sehen, welche Dateien betroffen sind.

## OpenCode-Thread starten

Ein `Thread` ist eine Unterhaltung mit einem Agenten.

So startest du einen OpenCode-Thread:

1. Öffne das Agent Panel.
2. Öffne das Menü für einen neuen Thread.
3. Wähle `OpenCode` als Agent aus.
4. Schreibe deinen ersten Prompt.

Guter erster Prompt:

```text
Schau dir dieses Projekt kurz an.
Erkläre mir in einfachen Worten, welche Dateien wichtig sind.
Ändere noch nichts.
```

Was bringt das?

Du gibst dem Agenten zuerst eine Analyseaufgabe statt sofort eine Bauaufgabe. Dadurch verstehst du besser, womit du arbeitest.

## Modell auswählen

OpenCode braucht ein KI-Modell im Hintergrund.

Je nach OpenCode-Konfiguration kannst du ein Modell oder einen Anbieter auswählen. Das kann zum Beispiel über OpenCode selbst, einen Login, einen API-Key oder eine Subscription laufen.

Typische Unterschiede zwischen Modellen:

- Einige Modelle sind schneller.
- Einige Modelle sind besser bei komplexen Aufgaben.
- Einige Modelle sind günstiger.
- Einige Modelle können längeren Kontext besser verarbeiten.
- Einige Modelle machen bessere Erklärungen.

Für Anfänger*innen gilt:

Starte mit dem Modell, das im Workshop empfohlen wird.

Wenn du später selbst auswählst, denke so:

| Situation | Sinnvolle Wahl |
| --- | --- |
| Kleine HTML/CSS-Aufgabe | schnelles Standardmodell |
| Fehler verstehen | Modell mit guten Erklärungen |
| Größere Änderung planen | stärkeres Modell |
| Viel Kontext im Projekt | Modell mit größerem Kontextfenster |

Was bringt das?

Die Modellwahl beeinflusst Qualität, Geschwindigkeit und manchmal Kosten. Für den Workshop ist wichtiger, dass du sauber arbeitest, als dass du sofort das "beste" Modell findest.

## Auth, Login und API-Keys

OpenCode kann nach einem Login oder API-Key fragen.

Ein `API-Key` ist ein geheimer Zugangsschlüssel für einen KI-Anbieter.

Wichtig:

- Teile API-Keys nie öffentlich.
- Schreibe API-Keys nicht in Projektdateien.
- Lade API-Keys nicht zu GitHub hoch.
- Wenn du keinen Zugang hast, warte auf die gemeinsame Erklärung im Workshop.

Was bringt das?

Ohne gültigen Zugang kann ein Agent oft nicht arbeiten. Gleichzeitig sind Zugangsdaten sensibel. Darum behandeln wir sie vorsichtig.

## Thread Panel und Thread History

Zed kann mehrere Agent-Threads verwalten.

Ein Thread ist sinnvoll für eine konkrete Aufgabe.

Beispiele:

```text
Thread 1: Projekt verstehen
Thread 2: Startseite bauen
Thread 3: Layout verbessern
Thread 4: Fehler beheben
```

Was bringt das?

Getrennte Threads halten den Kontext sauberer. Wenn ein Thread sehr lang wird, kann der Agent alte Entscheidungen durcheinanderbringen.

Für Anfänger*innen reicht:

- Nutze einen Thread pro größerem Arbeitsschritt.
- Starte einen neuen Thread, wenn das Thema wechselt.
- Lass dir am Ende eines Threads den Stand zusammenfassen.

Guter Abschlussprompt:

```text
Fasse zusammen:
1. Was wurde gebaut?
2. Welche Dateien wurden geändert?
3. Wie teste ich das Projekt?
4. Was ist der nächste sinnvolle Schritt?
```

## Kontext geben

Ein Agent arbeitet besser, wenn er weiß, worauf er achten soll.

Du kannst Kontext geben durch:

- klare Beschreibung deiner Idee
- Dateinamen
- ausgewählte Textstellen
- Fehlermeldungen
- Screenshots
- Links zu Referenzen
- Regeln aus deiner `AGENTS.md`

Schlechter Prompt:

```text
Mach die Seite besser.
```

Besser:

```text
Die Startseite wirkt zu textlastig.
Bitte schlage drei kleine visuelle Verbesserungen vor.
Ändere noch nichts.
Nutze nur HTML und CSS.
```

Was bringt das?

Je klarer der Kontext, desto weniger muss der Agent raten.

## Dateien erwähnen

Wenn du weißt, welche Datei wichtig ist, nenne sie direkt.

Beispiel:

```text
Schau dir `index.html` und `style.css` an.
Erkläre mir, wie die Seite aufgebaut ist.
Ändere noch nichts.
```

Was bringt das?

Der Agent konzentriert sich auf die relevanten Dateien und verliert weniger Zeit mit dem Rest des Projekts.

## Änderungen zuerst planen lassen

Bei größeren Änderungen solltest du OpenCode erst planen lassen.

Prompt:

```text
Bitte ändere noch nichts.
Analysiere zuerst das Projekt und schlage einen Plan in 3 bis 5 Schritten vor.
Nenne genau, welche Dateien du ändern würdest.
Warte danach auf meine Bestätigung.
```

Was bringt das?

Du behältst Kontrolle. Der Agent erklärt zuerst, was er tun will, bevor Dateien geändert werden.

## Kleine Änderungen erlauben

Wenn der Plan gut ist, gib eine kleine Aufgabe frei.

Beispiel:

```text
Setze nur Schritt 1 um.
Ändere nur `index.html` und `style.css`.
Erkläre danach kurz, was du geändert hast.
```

Was bringt das?

Kleine Änderungen sind leichter zu prüfen. Wenn etwas schiefgeht, findest du schneller die Ursache.

## Änderungen prüfen

Nach jeder Agent-Änderung solltest du prüfen:

1. Welche Dateien wurden geändert?
2. Passt die Änderung zur Aufgabe?
3. Funktioniert das Projekt noch?
4. Gibt es Fehlermeldungen?
5. Hat der Agent ungefragt zusätzliche Dinge eingebaut?

Nutze dafür:

- die geänderten Dateien in Zed
- das Git Panel
- den Project Diff
- den Browser
- Fehlermeldungen aus Terminal oder Konsole

Was bringt das?

Du übernimmst nicht blind KI-Code. Du lernst, den Prozess zu kontrollieren.

## Änderungen mit Git sichern

Wenn eine Änderung funktioniert, speichere sie mit Git.

Workflow:

```text
Änderung prüfen -> Commit schreiben -> Push zu GitHub
```

Beispiel für eine Commit-Nachricht:

```text
Add first prototype layout
```

Was bringt das?

Git ist dein Sicherheitsnetz. Wenn spätere Agent-Änderungen schlechter werden, hast du einen guten Zwischenstand gespeichert.

## Tool Permissions und Bestätigung

Ein Coding Agent kann je nach Einstellung Werkzeuge nutzen, zum Beispiel Dateien ändern oder Befehle ausführen.

Wenn Zed oder OpenCode fragt, ob eine Aktion erlaubt ist, lies kurz, was passieren soll.

Achte besonders auf:

- Welche Datei wird geändert?
- Wird ein Befehl ausgeführt?
- Werden neue Pakete installiert?
- Werden viele Dateien verändert?

Was bringt das?

Du vermeidest, dass der Agent zu viel auf einmal macht.

Gute Grenze:

```text
Füge keine neuen Libraries hinzu, ohne vorher zu fragen.
```

## Wenn OpenCode etwas falsch macht

Das passiert. Wichtig ist, wie du reagierst.

Nicht gut:

```text
Nein falsch, mach nochmal.
```

Besser:

```text
Die letzte Änderung hat das Layout verschlechtert.
Bitte erkläre zuerst, welche Änderung wahrscheinlich dafür verantwortlich ist.
Schlage dann den kleinsten möglichen Fix vor.
Ändere noch nichts.
```

Was bringt das?

Du zwingst den Agenten zur Analyse, statt direkt die nächste unsichere Änderung auszulösen.

## Wann du einen neuen Thread starten solltest

Starte einen neuen Thread, wenn:

- ein Thema abgeschlossen ist
- der Thread sehr lang geworden ist
- der Agent sich im Kreis dreht
- du mit einer neuen Aufgabe beginnst
- du eine saubere Zusammenfassung als Startpunkt willst

Guter Start für einen neuen Thread:

```text
Hier ist der aktuelle Stand:
[kurze Zusammenfassung einfügen]

Bitte schlage den nächsten kleinen Schritt vor.
Ändere noch nichts.
```

Was bringt das?

Ein neuer Thread reduziert alten Ballast. Das hilft dem Agenten, fokussierter zu arbeiten.

## Gute erste Prompts

Projekt verstehen:

```text
Schau dir dieses Projekt an.
Erkläre mir in einfachen Worten, welche Dateien wichtig sind.
Ändere nichts.
```

Plan erstellen:

```text
Ich möchte eine einfache Projektseite bauen.
Bitte schlage zuerst einen Plan in 3 bis 5 Schritten vor.
Ändere noch keine Dateien.
```

Kleine Änderung:

```text
Erstelle eine einfache Startseite mit Titel, kurzem Beschreibungstext und drei Karten.
Nutze nur HTML und CSS.
Ändere nur die notwendigen Dateien.
Erkläre danach, was du geändert hast.
```

Fehler erklären:

```text
Ich bekomme diese Fehlermeldung:

[Fehlermeldung einfügen]

Bitte erkläre sie in einfachen Worten.
Schlage den kleinsten möglichen Fix vor.
Ändere noch nichts.
```

## Mini-Glossar

| Begriff | Bedeutung |
| --- | --- |
| `OpenCode` | Coding Agent für die Arbeit an Softwareprojekten |
| `Agent Panel` | Zed-Bereich für Agent-Unterhaltungen |
| `Thread` | Eine einzelne Unterhaltung mit einem Agenten |
| `External Agent` | Externer Agent, der in Zed eingebunden wird |
| `ACP Registry` | Zed-Verzeichnis zum Installieren externer Agents |
| `Model` | KI-Modell, das Antworten und Code erzeugt |
| `API-Key` | Geheimer Zugangsschlüssel zu einem KI-Anbieter |
| `Context` | Informationen, die der Agent für die Aufgabe braucht |
| `Diff` | Anzeige der geänderten Stellen |

## Was du jetzt gelernt hast

Du weißt jetzt, wie OpenCode in Zed eingebunden wird und wie du einen OpenCode-Thread startest.

Du kennst die wichtigsten Optionen: Agent Panel, Threads, Modellwahl, Auth, Kontext, Tool-Bestätigungen und Git-Prüfung.

Der wichtigste Punkt: Lass OpenCode klein anfangen, prüfe jede Änderung und speichere gute Zwischenstände mit Git.
