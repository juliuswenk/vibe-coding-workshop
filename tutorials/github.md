---
layout: default
title: GitHub Tutorial
---

# GitHub Tutorial

In diesem Tutorial lernst du, wie du dein Projekt mit `Git` und `GitHub` sicherst.

Wir arbeiten hauptsächlich mit der Oberfläche von `Zed`, nicht mit Terminal-Befehlen. Das Ziel ist: Du sollst verstehen, was passiert, ohne direkt alle Git-Befehle auswendig zu lernen.

## Was diese Seite erklärt

Diese Seite erklärt:

- was `Git` ist
- was `GitHub` ist
- warum du beides beim Vibe Coding nutzen solltest
- welche Begriffe wichtig sind
- wie du ein Repository auf GitHub erstellst
- wie du es mit Zed auf deinen Rechner holst
- wie du Änderungen speicherst
- wie du Änderungen zu GitHub hochlädst

## Warum das für Vibe Coding wichtig ist

Wenn du mit einem `Coding Agent` arbeitest, können schnell viele Dateien geändert werden.

Das ist praktisch, aber auch riskant. Ein Agent kann:

- etwas kaputt machen
- zu viele Dateien ändern
- eine gute Version überschreiben
- eine Lösung komplizierter machen als nötig

`Git` ist dein Sicherheitsnetz. Es speichert Projektstände. Wenn etwas funktioniert, kannst du diesen Stand sichern. Wenn später etwas schiefgeht, kannst du sehen, was sich geändert hat.

---

## Git und GitHub kurz erklärt

`Git` ist ein Werkzeug auf deinem Computer. Es merkt sich Änderungen in deinem Projekt.

`GitHub` ist eine Website, auf der du dein Git-Projekt online speichern kannst.

## Die wichtigsten Begriffe

### Repository

Ein `Repository`, kurz `Repo`, ist ein Projektordner, der von Git verwaltet wird.

Beispiel:

```text
mein-erstes-projekt
```

Wenn dieser Ordner ein Git-Repository ist, kann Git Änderungen darin speichern.

### Clone

`Clone` bedeutet: Du kopierst ein GitHub-Repository auf deinen Computer. Dann ist es nicht mehr nur online, sondern du hast eine lokale Kopie.

Beispiel:

```text
GitHub Repo online -> Projektordner auf deinem Laptop
```

Danach kannst du lokal an den Dateien arbeiten.

### Commit

Ein `Commit` ist ein gespeicherter Projektstand.

Ein Commit braucht eine kurze Nachricht.

Gute Commit-Nachrichten:

```text
Add first homepage
```

```text
Change button colors
```

```text
Fix layout spacing
```

Schlechte Commit-Nachrichten:

```text
asdf
```

```text
changes
```

```text
final final wirklich final
```

### Stage

`Stage` bedeutet: Du wählst aus, welche Änderungen in den nächsten Commit sollen.

Beispiel:

- Du hast `index.html` geändert.
- Du hast `style.css` geändert.
- Du möchtest beide Änderungen speichern.
- Dann stagest du beide Dateien und machst danach einen Commit.

Für den Anfang gilt: Wenn du alleine arbeitest, kannst du meistens alle sinnvollen Änderungen gemeinsam stagen.

### Push

`Push` bedeutet: Du lädst deine lokalen Commits zu GitHub hoch.

Beispiel:

```text
Dein Laptop -> GitHub
```

Erst nach einem Push ist deine neue Version online auf GitHub sichtbar.

### Pull

`Pull` bedeutet: Du holst neue Änderungen von GitHub auf deinen Computer.

Beispiel:

```text
GitHub -> dein Laptop
```

Wenn du alleine arbeitest, brauchst du `Pull` seltener. Es ist trotzdem gut, vor dem Arbeiten kurz zu prüfen, ob GitHub neue Änderungen hat.

### Branch

Ein `Branch` ist eine eigene Entwicklungslinie in Git.

Für diesen Workshop bleiben wir auf `main`. Das ist der Haupt-Branch.

Branches werden später wichtig, wenn mehrere Menschen an einem Projekt arbeiten oder du größere Änderungen getrennt ausprobieren möchtest.

---

## Der einfache Solo-Workflow

Für den Anfang reicht dieser Ablauf:

1. Repository auf GitHub erstellen.
2. Repository mit Zed auf den Computer clonen.
3. Dateien in Zed ändern.
4. Änderungen im Git Panel prüfen.
5. Änderungen stagen. (Welche Änderungen sollen wirklich gespeichert werden?)
6. Commit mit kurzer Nachricht erstellen. (Die aktuelle Version auf deinem Computer speichern)
7. Push zu GitHub machen. (Die Version auf deinem Computer auf GitHub hochladen)

Kurz gesagt:

```text
Ändern -> Prüfen -> Commit (Speichern) -> Push (Hochladen)
```

## Repository erstellen und öffnen

### 1. Neues Repository auf GitHub erstellen

1. Öffne [github.com](https://github.com/).
2. Melde dich an.
3. Klicke oben rechts auf das `+`.
4. Wähle `New repository`.
5. Gib deinem Repository einen Namen.

Beispiel:

```text
mein-erstes-vibe-coding-projekt
```

6. Wähle `Public` oder `Private`.
7. Aktiviere `Add a README file`.
8. Klicke auf `Create repository`.

Für den Workshop ist `Private` völlig okay. `Public` bedeutet, dass andere Menschen dein Repository sehen können.

### 2. Repository-Adresse kopieren

Nach dem Erstellen siehst du dein neues Repository auf GitHub.

1. Klicke auf den grünen Button `Code`.
2. Wähle `HTTPS`.
3. Kopiere die Adresse.

Sie sieht ungefähr so aus:

```text
https://github.com/dein-name/mein-erstes-vibe-coding-projekt.git
```

Diese Adresse sagt Zed, welches Repository auf deinen Computer kopiert werden soll.

### 3. Repository in Zed clonen

Öffne `Zed`.

Dann:

1. Öffne die Command Palette.
   - macOS: `Cmd + Shift + P`
   - Windows: `Ctrl + Shift + P`
2. Suche nach `clone`.
3. Wähle die Git-Clone-Aktion aus.
4. Füge die GitHub-Adresse ein.
5. Wähle einen Ort auf deinem Computer aus, zum Beispiel deinen Projektordner.
6. Öffne das geklonte Projekt in Zed.

Wenn Zed dich fragt, ob du dich bei GitHub anmelden möchtest, folge dem Login-Flow.

Am Ende solltest du dein Projekt links im Dateibereich von Zed sehen.

---

## Erste Änderung speichern

### 4. Erste Änderung machen

Erstelle eine neue Datei in Zed.

Name:

```text
index.md
```

Inhalt:

```
Mein erstes Vibe-Coding-Projekt
```

Speichere die Datei.

Jetzt hat dein Projekt eine Änderung.

### 5. Git Panel in Zed öffnen

Das `Git Panel` zeigt dir, welche Dateien geändert wurden.

Du kannst es öffnen über:

- das Git-Symbol in der Statusleiste
- oder die Command Palette mit `git panel: toggle focus`

Im Git Panel solltest du jetzt `index.md` als geänderte oder neue Datei sehen.

Wenn du nichts siehst, prüfe:

- Ist die Datei gespeichert?
- Hast du wirklich das geklonte Repository geöffnet?
- Bist du im richtigen Projektordner?

### 6. Änderung prüfen

Bevor du etwas speicherst, schau dir die Änderung an.

In Zed kannst du dafür das Git Panel oder den `Project Diff` nutzen.

`Diff` bedeutet: Git zeigt dir den Unterschied zwischen dem alten und dem neuen Zustand.

Beispiel:

```text
Vorher: Datei existiert nicht.
Nachher: index.md wurde hinzugefügt.
```

Das ist wichtig, weil du gerade beim Vibe Coding nicht blind alles übernehmen solltest, was ein Agent geändert hat.

### 7. Änderung stagen

Im Git Panel kannst du Dateien auswählen, die in den nächsten Commit sollen.

Für den Anfang:

1. Suche `index.md` im Git Panel.
2. Setze das Häkchen neben der Datei.

Damit ist die Datei `staged`.

Das bedeutet: Diese Änderung wird gleich im nächsten Commit gespeichert.

### 8. Commit erstellen

Unten im Git Panel gibt es ein Feld für die Commit-Nachricht.

Schreibe:

```text
index.md hinzugefügt
```

Dann klicke auf den Commit-Button oder nutze die passende Tastenkombination, die Zed dir anzeigt.

Jetzt hast du deinen ersten Commit erstellt.

Das heißt: Git hat diesen Projektstand gespeichert.

### 9. Änderung zu GitHub pushen

Der Commit liegt jetzt erstmal nur auf deinem Computer.

Damit GitHub ihn bekommt, musst du `pushen`.

Im Git Panel gibt es dafür einen `Push`-Button. Du kannst auch über die Command Palette nach `git: push` suchen.

Nach dem Push:

1. Öffne dein Repository auf GitHub.
2. Lade die Seite neu.
3. Prüfe, ob `index.md` dort sichtbar ist.

Wenn ja: Du hast deine lokale Änderung erfolgreich zu GitHub hochgeladen.

---

## Weiterarbeiten und prüfen

### 10. Später weiterarbeiten

Wenn du später weiterarbeitest, nutze diesen Ablauf:

1. Öffne das Projekt in Zed.
2. Mache eine kleine Änderung.
3. Prüfe die Änderung im Git Panel.
4. Stage die passende Datei.
5. Schreibe eine klare Commit-Nachricht.
6. Committe.
7. Pushe.

Beispiel:

```text
Change homepage text
```

Oder:

```text
Add project cards
```

### 11. Wann du pull benutzt

Wenn du alleine arbeitest, passiert auf GitHub meistens nichts, was nicht vorher von deinem Computer kam.

Trotzdem ist `Pull` nützlich, wenn:

- du an einem anderen Computer gearbeitet hast
- du auf GitHub direkt eine Datei geändert hast
- später andere Menschen mitarbeiten

`Pull` holt Änderungen von GitHub zurück auf deinen Computer.

In Zed findest du `Pull` im Git Panel oder über die Command Palette mit `git: pull`.

---

### 12. Git und Coding Agents

Wenn ein Coding Agent Dateien ändert, schau danach ins Git Panel.

Frage dich:

- Welche Dateien wurden geändert?
- Passen diese Änderungen zur Aufgabe?
- Wurde etwas verändert, das gar nicht nötig war?
- Kann ich das Ergebnis öffnen oder testen?

Guter Prompt nach einer Agent-Änderung:

```text
Fasse mir kurz zusammen, welche Dateien du geändert hast und warum.
Ändere nichts weiter.
```

Wenn alles passt, machst du einen Commit.

Beispiel:

```text
Add first prototype layout
```

### 13. Zusammenarbeit kurz erwähnt

Git und GitHub sind auch für Zusammenarbeit gedacht.

Mehrere Menschen können an einem Projekt arbeiten, Änderungen teilen und später zusammenführen.

Das ist mächtig, aber für den Start auch mehr Komplexität. In diesem Workshop arbeiten wir erstmal alleine auf `main`.

Merke dir nur: Wenn du später mit anderen zusammenarbeitest, werden `Pull`, `Branches` und `Pull Requests` wichtiger.

## Mini-Glossar

| Begriff | Bedeutung |
| --- | --- |
| `Repository` | Ein Projektordner, der von Git verwaltet wird |
| `Clone` | Ein GitHub-Repository auf deinen Computer kopieren |
| `Stage` | Änderungen für den nächsten Commit auswählen |
| `Commit` | Einen Projektstand speichern |
| `Push` | Lokale Commits zu GitHub hochladen |
| `Pull` | Neue Änderungen von GitHub herunterladen |
| `Branch` | Eine eigene Entwicklungslinie in Git |
| `main` | Der Haupt-Branch deines Projekts |
| `Diff` | Anzeige, was sich geändert hat |

---

## Was du jetzt gelernt hast

Du weißt jetzt, was `Git` und `GitHub` sind und warum sie beim Vibe Coding wichtig sind.

Du kannst ein Repository auf GitHub erstellen, es mit Zed auf deinen Computer clonen, Änderungen prüfen, committen und zu GitHub pushen.

Das ist ein wichtiger Schritt: Du hast jetzt ein Sicherheitsnetz für deine Projekte.
