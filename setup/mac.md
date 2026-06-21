---
layout: default
title: Setup für macOS
---

# Setup für macOS

Diese Seite hilft dir dabei, deinen Mac für den Workshop vorzubereiten.

Du musst nicht verstehen, wie alle Werkzeuge im Detail funktionieren. Wichtig ist erst einmal: Am Ende kannst du Dateien bearbeiten, Projekte speichern und mit einem `Coding Agent` arbeiten.

## Was diese Seite erklärt

Du installierst und prüfst:

- einen GitHub-Account
- `Git`
- `Node.js LTS`
- `Zed`
- `OpenCode`
- einen einfachen Projektordner

## Warum das für Vibe Coding wichtig ist

Ein `Coding Agent` braucht einen Ort, an dem er arbeiten kann: einen Projektordner mit Dateien.

Damit dieser Arbeitsprozess gut funktioniert, brauchst du:

- einen Editor, um Dateien zu sehen und zu ändern
- `Git`, um Projektstände speichern zu können
- GitHub, um Projekte online abzulegen
- `Node.js`, damit einfache Webprojekte später laufen können
- `OpenCode`, damit du mit einem Coding Agent im Projekt arbeiten kannst

## Bevor du startest

Öffne diese Seite auf deinem Mac und arbeite die Schritte von oben nach unten durch.

Wenn ein Schritt nicht funktioniert: Nicht schlimm. Schreib dir die Fehlermeldung auf oder mach einen Screenshot. Genau solche Situationen gehören zum Arbeiten mit Entwicklungswerkzeugen dazu.

## 1. GitHub-Account erstellen

`GitHub` ist eine Website, auf der du Code speichern und teilen kannst. Für den Workshop brauchst du einen kostenlosen persönlichen Account.

1. Öffne [github.com](https://github.com/).
2. Klicke auf `Sign up`.
3. Erstelle einen Account mit deiner E-Mail-Adresse.
4. Bestätige deine E-Mail-Adresse.
5. Merke dir deinen Benutzernamen.

Du brauchst keinen bezahlten Plan.

Quelle: GitHub beschreibt in der offiziellen Anleitung, dass du für den Einstieg einen kostenlosen persönlichen Account mit bestätigter E-Mail-Adresse brauchst: [Creating an account on GitHub](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github).

## 2. Terminal öffnen

Das `Terminal` ist ein Programm, in dem du Textbefehle ausführst.

1. Drücke `Cmd + Leertaste`.
2. Tippe `Terminal`.
3. Drücke `Enter`.

Du siehst jetzt ein Fenster, in das du Befehle schreiben kannst.

## 3. Git prüfen oder installieren

`Git` speichert Versionen deines Projekts. Dadurch kannst du später nachvollziehen, was sich geändert hat.

Gib im Terminal ein:

```sh
git --version
```

Wenn eine Versionsnummer erscheint, ist `Git` installiert.

Wenn macOS fragt, ob es Command Line Tools installieren soll:

1. Bestätige die Installation.
2. Warte, bis sie fertig ist.
3. Öffne das Terminal neu.
4. Prüfe nochmal:

```sh
git --version
```

Falls das nicht funktioniert, lade `Git` über die offizielle Seite herunter: [git-scm.com/downloads](https://git-scm.com/downloads/).

## 4. Git einmal einrichten

Git soll wissen, welcher Name und welche E-Mail-Adresse zu deinen Änderungen gehören.

Ersetze die Beispielwerte durch deine Daten:

```sh
git config --global user.name "Dein Name"
git config --global user.email "deine-mail@example.com"
```

Prüfe danach:

```sh
git config --global user.name
git config --global user.email
```

Wenn dein Name und deine E-Mail-Adresse angezeigt werden, passt es.

## 5. Node.js LTS installieren

`Node.js` hilft uns später, einfache Webprojekte lokal auszuführen. `LTS` bedeutet: stabile Version für die meisten Nutzerinnen und Nutzer.

1. Öffne [nodejs.org](https://nodejs.org/).
2. Lade die `LTS`-Version für macOS herunter.
3. Öffne die heruntergeladene Datei.
4. Folge dem Installer.
5. Öffne danach das Terminal neu.

Prüfe die Installation:

```sh
node --version
npm --version
```

Wenn beide Befehle eine Versionsnummer anzeigen, ist alles bereit.

## 6. Zed installieren

`Zed` ist unser Code Editor. Darin öffnest und bearbeitest du Projektdateien.

1. Öffne [zed.dev/download](https://zed.dev/download).
2. Lade Zed für macOS herunter.
3. Öffne die heruntergeladene Datei.
4. Ziehe `Zed` in den Ordner `Programme`, falls macOS dich dazu auffordert.
5. Starte `Zed`.

Die offizielle Zed-Downloadseite zeigt die aktuelle Version und den macOS-Download: [Zed Download](https://zed.dev/download).

## 7. OpenCode installieren

`OpenCode` ist der Coding Agent, den wir im Workshop verwenden wollen. Er läuft im Terminal.

Installiere OpenCode mit `npm`:

```sh
npm install -g opencode-ai
```

Prüfe danach:

```sh
opencode --version
```

Wenn eine Versionsnummer erscheint, ist OpenCode installiert.

Die offizielle OpenCode-Dokumentation nennt `npm install -g opencode-ai` als Installationsmöglichkeit: [OpenCode Docs](https://opencode.ai/docs).

## 8. OpenCode verbinden

OpenCode braucht Zugriff auf ein KI-Modell. Je nach Workshop-Stand kann das über einen OpenCode-Account, einen API-Key oder einen anderen Provider laufen.

Für jetzt reicht:

1. Öffne das Terminal.
2. Starte OpenCode:

```sh
opencode
```

3. Wenn OpenCode dich zur Anmeldung oder Verbindung auffordert, folge den Anweisungen.
4. Wenn du nach einem API-Key gefragt wirst und noch keinen hast, warte auf die Erklärung im Workshop.

Du musst hier nichts kaufen, bevor wir gemeinsam geklärt haben, welchen Zugang wir verwenden.

## 9. Projektordner anlegen

Ein Projektordner ist einfach ein Ordner, in dem alle Dateien deines Projekts liegen.

Lege auf dem Schreibtisch einen Ordner an:

```sh
cd ~/Desktop
mkdir vibe-coding-projekte
cd vibe-coding-projekte
mkdir erstes-projekt
cd erstes-projekt
```

Prüfe, wo du bist:

```sh
pwd
```

Du solltest einen Pfad sehen, der ungefähr so endet:

```text
Desktop/vibe-coding-projekte/erstes-projekt
```

## 10. Projekt in Zed öffnen

Öffne `Zed`.

Dann:

1. Klicke auf `File`.
2. Klicke auf `Open Folder`.
3. Wähle den Ordner `erstes-projekt`.
4. Öffne ihn.

Du siehst jetzt deinen Projektordner in Zed. Er ist noch leer. Das ist normal.

## 11. Kurzer Funktionstest

Gehe im Terminal in deinen Projektordner:

```sh
cd ~/Desktop/vibe-coding-projekte/erstes-projekt
```

Starte OpenCode:

```sh
opencode
```

Wenn OpenCode startet, bist du bereit für den Workshop.

Wenn OpenCode nicht startet, prüfe:

- Ist `Node.js` installiert?
- Gibt `npm --version` eine Versionsnummer aus?
- Gibt `opencode --version` eine Versionsnummer aus?
- Bist du im richtigen Ordner?

## Was du jetzt gelernt hast

Du hast deinen Mac so vorbereitet, dass du mit einem Coding Agent an einem eigenen Projekt arbeiten kannst.

Du hast außerdem gesehen, dass ein Projekt nicht mit Code beginnt, sondern mit einer einfachen Arbeitsumgebung: Account, Editor, Terminal, Projektordner und Agent.
