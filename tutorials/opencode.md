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

Wenn du OpenCode in Zed nutzt, arbeitest du direkt im Projekt. Das bedeutet:

- Der Agent kann deine Dateien sehen.
- Du kannst Änderungen direkt prüfen.
- Du kannst Git nutzen, um gute Zwischenstände zu speichern.
- Du kannst in kleinen Schritten weiterarbeiten.

---

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

---

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

---

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

---

## Modell auswählen

OpenCode braucht ein KI-Modell im Hintergrund.

Je nach OpenCode-Konfiguration kannst du ein Modell auswählen.

Typische Unterschiede zwischen Modellen:

- Einige Modelle sind schneller.
- Einige Modelle sind besser bei komplexen Aufgaben.
- Einige Modelle können längeren Kontext besser verarbeiten.
- Einige Modelle machen bessere Erklärungen.

Für Anfänger*innen gilt:

Was bringt das?

Die Modellwahl beeinflusst Qualität, Geschwindigkeit und manchmal Kosten. Für den Workshop ist wichtiger, dass du sauber arbeitest, als dass du sofort das "beste" Modell findest.

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

---

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

---

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

## Was du jetzt gelernt hast

Du weißt jetzt, wie OpenCode in Zed eingebunden wird und wie du einen OpenCode-Thread startest.

Du kennst die wichtigsten Optionen: Agent Panel, Threads, Modellwahl, Auth, Kontext, Tool-Bestätigungen und Git-Prüfung.

Der wichtigste Punkt: Lass OpenCode klein anfangen, prüfe jede Änderung und speichere gute Zwischenstände mit Git.
