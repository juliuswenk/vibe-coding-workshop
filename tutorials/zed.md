---
layout: default
title: Zed Tutorial
---

# Zed Tutorial

In diesem Tutorial lernst du, was `Zed` ist und wie du dich in der Oberfläche zurechtfindest.

Zed ist das Programm, in dem du deine Projektdateien öffnest, bearbeitest, mit Git arbeitest und später deinen Coding Agent nutzt.

## Was diese Seite erklärt

Diese Seite erklärt:

- was ein Code Editor ist
- was eine `IDE` ist
- warum wir Zed im Workshop nutzen
- wie Zed grob aufgebaut ist
- welche Bereiche der Oberfläche wichtig sind
- wie du ein Projekt öffnest
- wie du Dateien erstellst und bearbeitest
- wo du Git und Agent-Funktionen findest

## Warum das für Vibe Coding wichtig ist

Beim Vibe Coding arbeitest du nicht nur in einem Chatfenster.

Du brauchst eine Umgebung, in der du:

- Dateien sehen kannst
- Änderungen prüfen kannst
- Code oder Text bearbeiten kannst
- dein Projekt starten oder testen kannst
- mit Git speichern kannst
- mit einem Coding Agent im Projekt arbeiten kannst

Zed ist diese Arbeitsumgebung. Wenn du Zed grob verstehst, kannst du besser nachvollziehen, was ein Agent in deinem Projekt verändert.

## Was ist ein Code Editor?

Ein `Code Editor` ist ein Programm zum Bearbeiten von Code- und Textdateien.

Du kannst ihn dir wie einen sehr spezialisierten Texteditor vorstellen.

Ein normaler Texteditor kann Text schreiben. Ein Code Editor kann zusätzlich:

- Projektordner anzeigen
- Code farbig markieren
- Fehler sichtbar machen
- Dateien schnell suchen
- Git-Änderungen anzeigen
- ein Terminal öffnen
- mit Coding Agents verbunden werden

Beispiele für Code Editoren sind:

- `Zed`
- `Visual Studio Code`
- `Sublime Text`
- `Atom`

## Was ist eine IDE?

`IDE` steht für `Integrated Development Environment`.

Auf Deutsch: integrierte Entwicklungsumgebung.

Eine IDE bündelt mehrere Werkzeuge, die man zum Programmieren braucht:

- Editor
- Dateiansicht
- Terminal
- Git-Werkzeuge
- Fehlermeldungen
- Projektverwaltung
- manchmal Debugger oder Build-Werkzeuge

Für Anfänger*innen ist der Unterschied zwischen `Code Editor` und `IDE` nicht entscheidend.

Wichtig ist: Zed ist der Ort, an dem dein Projekt sichtbar und bearbeitbar wird.

## Warum Zed?

Wir nutzen Zed, weil es für den Workshop genug kann, aber nicht zu überladen wirkt.

Zed bietet:

- eine klare Oberfläche
- schnellen Zugriff auf Projektdateien
- integrierte Git-Funktionen
- ein eingebautes Terminal
- ein Agent Panel für KI-Unterstützung
- gute Unterstützung für moderne Webprojekte

Du musst nicht jede Funktion kennen. Für den Workshop reichen die Grundlagen.

## Die wichtigsten Bereiche in Zed

Zed besteht grob aus diesen Bereichen:

```text
Projektdateien links | Editor in der Mitte | Panels unten/seitlich
```

Je nach Fenstergröße oder Einstellung können Panels an anderen Stellen erscheinen. Das ist normal.

## 1. Project Panel

Das `Project Panel` zeigt die Dateien und Ordner deines Projekts.

Typische Dinge, die du dort machst:

- Dateien öffnen
- neue Dateien erstellen
- Ordner erstellen
- Dateien umbenennen
- sehen, welche Dateien zum Projekt gehören

Beispiel:

```text
mein-projekt
├── index.html
├── style.css
└── README.md
```

Wenn du eine Datei anklickst, öffnet sie sich im Editor.

## 2. Editor-Bereich

Der Editor ist der große Bereich in der Mitte.

Hier bearbeitest du Dateien.

Beispiel:

```html
<h1>Mein Projekt</h1>
<p>Das ist meine erste Seite.</p>
```

Zed hebt Code farbig hervor. Das nennt man `Syntax Highlighting`.

Das hilft dir zu erkennen:

- Was ist Text?
- Was ist ein HTML-Tag?
- Was ist ein Dateiname?
- Was ist vielleicht ein Fehler?

## 3. Tabs

Wenn du mehrere Dateien öffnest, erscheinen sie als Tabs.

Beispiel:

```text
index.html | style.css | README.md
```

Ein Tab ist wie ein geöffneter Dokument-Reiter im Browser.

Du kannst zwischen Dateien wechseln, ohne sie jedes Mal neu suchen zu müssen.

## 4. Command Palette

Die `Command Palette` ist eine Suchfunktion für Zed-Befehle.

Du öffnest sie mit:

- macOS: `Cmd + Shift + P`
- Windows: `Ctrl + Shift + P`

Danach kannst du nach Aktionen suchen.

Beispiele:

```text
git panel
```

```text
agent: new thread
```

```text
zed: acp registry
```

Wenn du nicht weißt, wo eine Funktion ist, ist die Command Palette oft der schnellste Weg.

## 5. Terminal

Das `Terminal` ist ein Bereich, in dem du Textbefehle ausführen kannst.

In Zed kannst du ein Terminal direkt im Projekt öffnen.

Das ist praktisch, weil du dann nicht zwischen vielen Fenstern wechseln musst.

Beispiele für Befehle:

```text
node --version
```

```text
opencode --version
```

```text
git status
```

Für den Start musst du nicht viele Befehle kennen. Aber du solltest wissen, dass das Terminal existiert.

## 6. Git Panel

Das `Git Panel` zeigt dir, welche Dateien sich geändert haben.

Du nutzt es, um:

- Änderungen anzuschauen
- Dateien zu stagen
- Commits zu erstellen
- Änderungen zu GitHub zu pushen
- Änderungen von GitHub zu pullen

Beim Vibe Coding ist das besonders wichtig, weil ein Coding Agent mehrere Dateien ändern kann.

Nach Agent-Änderungen solltest du immer kurz ins Git Panel schauen.

Frage dich:

- Welche Dateien wurden geändert?
- Passt das zur Aufgabe?
- Wurde etwas Unerwartetes geändert?

## 7. Project Diff

Ein `Diff` zeigt dir den Unterschied zwischen vorher und nachher.

Beispiel:

```text
- alter Text
+ neuer Text
```

Das Minus bedeutet: Diese Zeile wurde entfernt.

Das Plus bedeutet: Diese Zeile wurde hinzugefügt.

Der Project Diff ist nützlich, wenn du vor einem Commit prüfen willst, was wirklich verändert wurde.

## 8. Agent Panel

Das `Agent Panel` ist der Bereich, in dem du mit einem Coding Agent arbeitest.

Du kannst dort zum Beispiel:

- Fragen zu deinem Projekt stellen
- Dateien erklären lassen
- kleine Änderungen planen lassen
- Änderungen durchführen lassen
- Fehlermeldungen erklären lassen

Guter erster Prompt:

```text
Schau dir dieses Projekt kurz an.
Erkläre mir in einfachen Worten, welche Dateien wichtig sind.
Ändere noch nichts.
```

Wichtig: Lass den Agenten nicht sofort alles bauen. Starte klein.

## 9. Ein Projekt öffnen

Ein Projekt ist meistens einfach ein Ordner.

Um ein Projekt in Zed zu öffnen:

1. Öffne `Zed`.
2. Klicke auf `File`.
3. Wähle `Open Folder`.
4. Wähle deinen Projektordner.
5. Öffne ihn.

Danach sollte der Ordner links im Project Panel sichtbar sein.

## 10. Eine Datei erstellen

Im Project Panel:

1. Rechtsklick auf deinen Projektordner.
2. Wähle `New File`.
3. Gib einen Dateinamen ein.

Beispiel:

```text
index.html
```

Dann kannst du die Datei im Editor bearbeiten.

## 11. Eine Datei speichern

Normalerweise speichert Zed automatisch oder zeigt ungespeicherte Änderungen an.

Für den Anfang kannst du bewusst speichern:

- macOS: `Cmd + S`
- Windows: `Ctrl + S`

Wenn du unsicher bist: Speichere einmal, bevor du testest oder committest.

## 12. Eine Datei suchen

In echten Projekten entstehen schnell mehrere Dateien.

Du kannst Dateien suchen mit:

- macOS: `Cmd + P`
- Windows: `Ctrl + P`

Dann tippst du den Dateinamen ein.

Beispiel:

```text
style.css
```

## 13. Typischer Workshop-Workflow in Zed

Für den Workshop reicht dieser Ablauf:

1. Projektordner in Zed öffnen.
2. Kurz anschauen, welche Dateien existieren.
3. Coding Agent nach einem kleinen Plan fragen.
4. Eine kleine Änderung machen lassen.
5. Ergebnis prüfen.
6. Git Panel öffnen.
7. Änderungen anschauen.
8. Commit erstellen, wenn es funktioniert.

Kurz:

```text
Öffnen -> Planen -> Ändern -> Prüfen -> Committen
```

## 14. Was du nicht sofort verstehen musst

Du musst am Anfang nicht verstehen:

- alle Einstellungen
- alle Tastenkürzel
- Debugging
- Worktrees
- komplexe Git-Funktionen
- alle Agent-Profile
- jede Fehlermeldung

Das kommt später, wenn du es wirklich brauchst.

Für den Start reicht:

- Projekt öffnen
- Dateien finden
- Dateien bearbeiten
- Git Panel öffnen
- Agent Panel öffnen
- kleine Änderungen prüfen

## 15. Wenn du dich verirrst

Wenn Zed unübersichtlich wird:

1. Schließe unnötige Tabs.
2. Öffne den Projektordner neu.
3. Suche Dateien mit `Cmd + P` oder `Ctrl + P`.
4. Öffne die Command Palette und suche nach der Funktion.
5. Frage den Coding Agent:

```text
Ich bin in Zed gerade unsicher.
Erkläre mir, welche Datei ich öffnen soll und warum.
Ändere nichts.
```

## Mini-Glossar

| Begriff | Bedeutung |
| --- | --- |
| `Code Editor` | Programm zum Bearbeiten von Code- und Textdateien |
| `IDE` | Entwicklungsumgebung mit mehreren Werkzeugen an einem Ort |
| `Project Panel` | Dateiansicht deines Projekts |
| `Editor` | Bereich, in dem du Dateien bearbeitest |
| `Tab` | Geöffnete Datei im Editor |
| `Command Palette` | Suche für Zed-Befehle |
| `Terminal` | Bereich für Textbefehle |
| `Git Panel` | Bereich für Git-Änderungen |
| `Project Diff` | Ansicht der Änderungen |
| `Agent Panel` | Bereich für den Coding Agent |

## Was du jetzt gelernt hast

Du weißt jetzt, was Zed ist, was eine IDE grob bedeutet und welche Bereiche der Oberfläche für den Workshop wichtig sind.

Du kannst ein Projekt öffnen, Dateien finden, neue Dateien erstellen, das Git Panel finden und das Agent Panel einordnen.

Das ist genug, um im Workshop nicht nur Prompts zu schreiben, sondern wirklich am eigenen Projekt zu arbeiten.
