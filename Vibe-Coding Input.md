---
layout: default
title: Vibe-Coding Input
permalink: /theorie/
---

# Vibe-Coding Input

Vibe Coding bedeutet: Du beschreibst einem `Coding Agent`, was du bauen möchtest, und entwickelst gemeinsam mit ihm ein funktionierendes Projekt.

Du schreibst nicht jede Codezeile selbst. Deine Aufgabe ist es, Ziele zu formulieren, Entscheidungen zu treffen, Ergebnisse zu prüfen und gutes Feedback zu geben.

## Was diese Seite erklärt

Diese Seite erklärt die wichtigsten Grundlagen für den Workshop:

- was `Vibe Coding` bedeutet
- was Vibe Coding gut kann
- wo die Grenzen liegen
- wie gute Prompts aussehen
- wie du mit OpenCode und Zed arbeitest
- wie du Ergebnisse prüfst
- wie du mit Fehlern umgehst
- wie du klare Grenzen setzt
- wie eine `AGENTS.md`-Datei hilft
- wie du externe Referenzen sinnvoll nutzt
- welche fortgeschrittenen Arbeitsweisen später wichtig werden

## Warum das für Vibe Coding wichtig ist

Vibe Coding funktioniert nicht dadurch, dass du einer KI einfach sagst: "Bau mir eine App."

Gute Ergebnisse entstehen, wenn du den Prozess führst:

- Du beschreibst eine kleine Aufgabe.
- Du lässt dir einen Plan erklären.
- Du erlaubst eine Änderung.
- Du prüfst das Ergebnis.
- Du gibst konkretes Feedback.
- Du machst den nächsten kleinen Schritt.

Der `Coding Agent` ist ein Werkzeug. Er kann dir viel Arbeit abnehmen, aber du bleibst verantwortlich für Richtung, Entscheidungen und Kontrolle.

## Inhaltsübersicht

1. Was Vibe Coding ist
2. Was Vibe Coding gut kann
3. Wo Vibe Coding begrenzt ist
4. Die wichtigste Regel
5. Gute Prompts für den Start
6. OpenCode in Zed
7. Was du immer prüfen solltest
8. Gute Aufgaben für Anfänger*innen
9. Fehler als Teil des Workflows
10. Grenzen setzen
11. Externe Referenzen nutzen
12. `AGENTS.md` als Projektanleitung
13. Fortgeschritten: AI Development Guide
14. Fortgeschritten: Projekt in Phasen aufteilen
15. Fortgeschritten: Erst fragen, dann bauen
16. Fortgeschritten: Agenten nicht alles glauben
17. Fortgeschritten: Git als Sicherheitsnetz
18. Gute Abschlussfrage nach jeder Session

## 1. Was Vibe Coding ist

Vibe Coding heißt: Du arbeitest mit einem Coding Agent an einem Softwareprojekt, ohne alles selbst von Hand schreiben zu müssen.

Das kann sehr schnell sein. Es kann aber auch chaotisch werden, wenn du:

- zu viel auf einmal verlangst
- Ergebnisse nicht prüfst
- nicht nachfragst, was geändert wurde
- dem Agenten keine Grenzen setzt

Für diesen Kurs heißt Vibe Coding nicht: "Die KI macht alles."

Es heißt: Du benutzt einen Agenten als technisches Werkzeug, um Ideen schneller auszuprobieren, Prototypen zu bauen und deinen eigenen Lernprozess zu unterstützen.

## 2. Was Vibe Coding gut kann

Vibe Coding ist besonders stark bei:

- schnellen Prototypen
- kleinen Webseiten
- interaktiven Skizzen
- einfachen Tools
- Erklärungen zu bestehenden Dateien
- Übersetzungen von Fehlermeldungen
- kleinen Feature-Ergänzungen
- Layout, Text, Struktur und Styling
- dem Zerlegen von Code in kleinere Schritte
- dem Vergleichen von Alternativen
- Dokumentation und Setup-Anleitungen

Ein guter Coding Agent kann Dateien lesen, Änderungen vorschlagen, Code ausführen und Fehlermeldungen nutzen, um weiterzuarbeiten.

Dadurch fühlt sich der Prozess oft eher wie ein Gespräch über ein Projekt an als wie klassisches Programmieren.

## 3. Wo Vibe Coding begrenzt ist

Coding Agents machen Fehler. Sie können überzeugend klingen und trotzdem falschen Code schreiben.

Typische Probleme:

- Der Agent baut mehr als du gefragt hast.
- Der Agent verändert bestehende Logik, obwohl es nicht nötig ist.
- Der Agent erfindet Libraries, Funktionen oder APIs.
- Der Agent übersieht Nebenwirkungen.
- Der Agent macht Code komplizierter als nötig.
- Der Agent löst ein Symptom, aber nicht die eigentliche Ursache.
- Der Agent kann Sicherheitsprobleme einbauen.
- Der Agent kann bei großen Projekten den Überblick verlieren.

Vibe Coding funktioniert deshalb nur gut, wenn du den Prozess führst.

Du musst nicht jede Codezeile verstehen. Du solltest aber immer wissen:

- Was soll das Projekt tun?
- Was wurde gerade geändert?
- Wie kann ich testen, ob es funktioniert?
- Was soll der Agent als Nächstes machen?

## 4. Die wichtigste Regel

Arbeite in kleinen Schritten.

Schlecht:

```text
Baue mir eine komplette interaktive Website mit Login, Datenbank, Galerie, Animationen und Exportfunktion.
```

Besser:

```text
Erstelle eine einfache Startseite mit einem Titel, einem kurzen Beschreibungstext und einem Button.
Nutze nur HTML und CSS.
Danach zeige mir, welche Dateien du geändert hast.
```

Wenn das funktioniert, kommt der nächste Schritt.

## 5. Gute Prompts für den Start

Ein guter Prompt enthält meistens:

- Ziel
- Kontext
- Einschränkungen
- gewünschtes Ergebnis
- Prüfschritt

Beispiel:

```text
Ich möchte eine kleine Webseite für eine interaktive Installation bauen.
Erstelle eine einfache HTML/CSS-Version mit einem Titel, einem kurzen Introtext und drei Projektkarten.
Nutze keine externen Frameworks.
Ändere nur Dateien in diesem Ordner.
Erkläre danach kurz, was du geändert hast und wie ich es im Browser öffnen kann.
```

Noch besser ist es, wenn du zuerst planen lässt:

```text
Ich möchte eine kleine Webseite bauen, kenne mich aber kaum mit Code aus.
Bitte schlage zuerst einen kurzen Plan in 3 bis 5 Schritten vor.
Ändere noch keine Dateien.
```

## 6. OpenCode in Zed

In diesem Workshop arbeitest du mit `Zed` als Code Editor und `OpenCode` als Coding Agent.

Ein sinnvoller Ablauf:

1. Öffne dein Projekt in Zed.
2. Öffne den Projektordner im Terminal.
3. Starte OpenCode.
4. Beschreibe eine kleine Aufgabe.
5. Lass dir zuerst den Plan erklären.
6. Erlaube die Änderung.
7. Prüfe das Ergebnis.
8. Gib konkretes Feedback.

Beispiel für den ersten Prompt:

```text
Schau dir dieses Projekt kurz an.
Erkläre mir in einfachen Worten, welche Dateien für den Einstieg wichtig sind.
Ändere noch nichts.
```

Beispiel für eine kleine Änderung:

```text
Erstelle eine sehr einfache HTML-Seite für ein Projekt namens "Black Box Breakout".
Sie soll einen Titel, einen kurzen Beschreibungstext und drei farbige Bereiche haben.
Nutze nur HTML und CSS.
Bitte ändere nur die Dateien, die dafür notwendig sind.
```

Beispiel für Feedback:

```text
Das ist zu textlastig.
Mach die Seite visueller, aber behalte die bestehende Struktur.
Bitte ändere nur das CSS.
```

## 7. Was du immer prüfen solltest

Nach jeder Änderung:

1. Welche Dateien wurden geändert?
2. Kann ich das Projekt starten oder öffnen?
3. Sieht das Ergebnis ungefähr so aus, wie ich wollte?
4. Gibt es Fehlermeldungen?
5. Hat der Agent ungefragt zusätzliche Dinge eingebaut?

Wenn etwas unklar ist, frage:

```text
Erkläre mir die letzte Änderung in einfachen Worten.
Welche Datei ist am wichtigsten?
Welche Zeilen sollte ich mir anschauen?
```

## 8. Gute Aufgaben für Anfänger*innen

Starte mit Aufgaben, die sichtbar und überschaubar sind:

- eine einfache Webseite erstellen
- Farben und Layout ändern
- Textbereiche ergänzen
- Buttons oder Karten bauen
- eine kleine Interaktion hinzufügen
- einen Fehler aus der Konsole erklären lassen
- eine README schreiben lassen
- eine vorhandene Datei zusammenfassen lassen

Vermeide am Anfang:

- Login-Systeme
- Datenbanken
- Bezahlsysteme
- komplexe Installationen
- große Refactorings
- mehrere Frameworks gleichzeitig
- Sicherheitsfunktionen, die du nicht verstehst

## 9. Fehler sind Teil des Workflows

Wenn etwas nicht funktioniert, kopiere nicht einfach blind neue Prompts hinterher.

Gib dem Agenten die Fehlermeldung und den Kontext.

Beispiel:

```text
Beim Starten bekomme ich diese Fehlermeldung:

[Fehlermeldung hier einfügen]

Bitte erkläre zuerst, was sie bedeutet.
Schlage dann den kleinsten möglichen Fix vor.
Ändere noch nichts, bevor du den Plan erklärt hast.
```

Wenn der Agent schon etwas geändert hat und es schlechter wurde:

```text
Die letzte Änderung hat das Layout kaputt gemacht.
Bitte analysiere, welche Änderung wahrscheinlich dafür verantwortlich ist.
Schlage eine minimale Korrektur vor.
```

## 10. Grenzen setzen

Coding Agents arbeiten besser, wenn du klare Grenzen setzt.

Nützliche Einschränkungen:

```text
Ändere nur HTML und CSS.
```

```text
Füge keine neuen Abhängigkeiten hinzu.
```

```text
Erstelle zuerst einen Plan und warte auf meine Bestätigung.
```

```text
Halte die Lösung so einfach wie möglich.
```

```text
Erkläre mir am Ende, wie ich das Ergebnis testen kann.
```

## 11. Externe Referenzen nutzen

Du darfst externe Beispiele nutzen. Das ist sogar oft sinnvoll.

Beispiele:

- `three.js` Demos
- CodePen-Beispiele
- GitHub-Repositories
- Dokumentationen
- Screenshots von Layouts
- kleine Animationen oder Interaktionsideen

Wichtig ist: Eine Referenz ist kein fertiger Arbeitsauftrag.

Schlecht:

```text
Bau mir diese Three.js-Demo nach.
```

Besser:

```text
Ich mag an dieser Three.js-Demo die langsam rotierende 3D-Form und die dunkle Bühne.
Bitte baue eine sehr einfache eigene Version davon.
Nutze nur eine Kugel, eine Lichtquelle und eine Kamera.
Erstelle zuerst einen Plan und sage mir, welche Dateien du ändern würdest.
```

Wenn du eine externe Referenz nutzt, beschreibe:

- Was genau gefällt dir daran?
- Was soll übernommen werden?
- Was soll nicht übernommen werden?
- Wie einfach soll die erste Version sein?
- Darf der Agent eine Library nutzen?

Bei Libraries wie `three.js` ist besonders wichtig:

- Starte mit einem kleinen Demo.
- Nutze die offizielle Dokumentation oder ein kleines Beispiel.
- Lass dir erklären, welche Dateien neu sind.
- Teste nach jeder Änderung im Browser.
- Verlange keine komplette 3D-Welt im ersten Prompt.

Guter Prompt:

```text
Ich möchte eine kleine Three.js-Szene als Experiment bauen.
Die Szene soll nur einen rotierenden Würfel auf dunklem Hintergrund zeigen.
Nutze eine möglichst einfache Struktur.
Erkläre mir zuerst, welche Dateien nötig sind.
Ändere noch nichts, bevor du den Plan gezeigt hast.
```

## 12. AGENTS.md als Projektanleitung

Eine `AGENTS.md`-Datei ist eine Anleitung für den Coding Agent.

Sie sagt dem Agenten, wie er in einem Projekt arbeiten soll. Das ist hilfreich, weil Agents sonst oft raten, welche Regeln gelten.

Eine gute `AGENTS.md` kann enthalten:

- Was ist das Ziel des Projekts?
- Welche Dateien sind wichtig?
- Wie startet man das Projekt?
- Wie testet man das Projekt?
- Welche Designregeln gelten?
- Welche Dateien darf der Agent ändern?
- Welche Dateien soll der Agent nicht anfassen?
- Wie einfach soll die Lösung bleiben?
- Wann soll der Agent erst fragen?

Beispiel:

```md
# AGENTS.md

Dieses Projekt ist ein kleiner Prototyp für eine interaktive Installation.

## Arbeitsweise

- Mache kleine, verständliche Änderungen.
- Erkläre vor größeren Änderungen zuerst deinen Plan.
- Füge keine neuen Libraries hinzu, ohne zu fragen.
- Ändere keine Setup-Dateien, außer es ist wirklich nötig.

## Testen

- Öffne `index.html` im Browser.
- Prüfe, ob Text und Buttons sichtbar sind.
- Prüfe die Browser-Konsole auf Fehler.

## Design

- Halte das Layout einfach.
- Nutze klare Kontraste.
- Keine überladenen Animationen.
```

Eine `AGENTS.md` macht den Agenten nicht perfekt. Sie reduziert aber Missverständnisse.

Für den Workshop gilt: Wenn dein eigenes Projekt größer wird, ist eine kleine `AGENTS.md` oft besser als ein sehr langer Prompt.

## 13. Fortgeschritten: AI Development Guide

Bei größeren Projekten lohnt es sich, dem Agenten eine feste Projektanleitung zu geben.

Das kann eine Datei wie diese sein:

- `AGENTS.md`
- `AI_DEVELOPMENT_GUIDE.md`
- `CONTRIBUTING.md`

Für Anfänger*innen reicht meistens `AGENTS.md`, weil viele Coding Agents diese Datei automatisch beachten.

Der wichtigste Inhalt ist nicht die perfekte Form, sondern klare Regeln:

- Was bauen wir?
- Was ist gerade nicht Teil des Projekts?
- Welche Befehle testen das Projekt?
- Was soll einfach bleiben?
- Wann muss der Agent fragen?

## 14. Fortgeschritten: Projekt in Phasen aufteilen

Für größere Projekte solltest du nicht alles in einem Thread bauen.

Teile das Projekt in Phasen:

1. Konzept
2. Grundstruktur
3. Erste sichtbare Version
4. Interaktion
5. Styling
6. Tests
7. Aufräumen
8. Dokumentation

Für jede Phase kannst du einen eigenen Agent-Thread starten. Das hält den Kontext sauberer und verhindert, dass alte Entscheidungen den nächsten Schritt verwirren.

## 15. Fortgeschritten: Erst fragen, dann bauen

Bei größeren Änderungen ist dieser Prompt nützlich:

```text
Bitte ändere noch nichts.
Analysiere zuerst das Projekt und schlage einen Plan für die nächste Änderung vor.
Nenne genau, welche Dateien du ändern würdest.
Warte danach auf meine Bestätigung.
```

Das gibt dir Kontrolle zurück.

## 16. Fortgeschritten: Agenten nicht alles glauben

Wenn ein Agent eine technische Entscheidung trifft, frage nach dem Grund:

```text
Warum hast du diese Lösung gewählt?
Welche einfachere Alternative gäbe es?
Welche Nachteile hat deine Lösung?
```

Gerade bei Anfänger*innen ist das wichtig, weil Agents oft zu komplexe Lösungen vorschlagen.

Einfacher Code ist meistens besser für den Lernprozess.

## 17. Fortgeschritten: Git als Sicherheitsnetz

`Git` speichert Projektstände. Wenn du mit Coding Agents arbeitest, ist das besonders wichtig.

Gute Gewohnheit:

1. Starte mit einem funktionierenden Zustand.
2. Lass den Agenten eine kleine Änderung machen.
3. Teste.
4. Wenn es gut ist, speichere den Stand mit Git.

Nützliche Befehle:

```sh
git status
git diff
git add .
git commit -m "Add first prototype"
```

Wenn du noch nicht sicher mit Git bist, frage den Agenten:

```text
Erkläre mir, was `git status` gerade bedeutet.
Ändere nichts.
```

## 18. Gute Abschlussfrage nach jeder Session

Beende eine Vibe-Coding-Session nicht einfach, sobald etwas funktioniert.

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

## Kurzfassung

Vibe Coding ist gut für schnelle Prototypen und kreative Experimente. Es ersetzt aber nicht dein Urteilsvermögen.

Arbeite klein, prüfe oft, setze klare Grenzen und lass dir Änderungen erklären. Je größer das Projekt wird, desto wichtiger werden Projektregeln, Tests, Git und klare Phasen.

## Was du jetzt gelernt hast

Du weißt jetzt, wie du mit einem Coding Agent arbeitest, ohne die Kontrolle über dein Projekt abzugeben.

Du hast gelernt, wie gute Prompts aufgebaut sind, warum kleine Schritte wichtig sind, wie du Fehler nutzt, wie externe Referenzen helfen können und wie eine `AGENTS.md` dem Agenten klare Projektregeln gibt.
