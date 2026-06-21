---
layout: default
title: Setup für macOS
---

# Setup für macOS

Diese Seite hilft dir dabei, deinen Mac für den Workshop vorzubereiten.

Wir nutzen `Homebrew` als Package Manager. Ein Package Manager installiert Programme über Befehle im Terminal. Das wirkt am Anfang ungewohnt, ist aber oft einfacher als viele einzelne Downloadseiten.

## Was diese Seite erklärt

Du installierst und prüfst:

- einen GitHub-Account
- `Homebrew`
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

---

## Bevor du startest

Öffne diese Seite auf deinem Mac und arbeite die Schritte von oben nach unten durch.

Wenn ein Schritt nicht funktioniert: Nicht schlimm. Schreib dir die Fehlermeldung auf oder mach einen Screenshot.

## Installation und Einrichtung

### 1. GitHub-Account erstellen

`GitHub` ist eine Website, auf der du Code speichern und teilen kannst. Für den Workshop brauchst du einen kostenlosen persönlichen Account.

1. Öffne [github.com](https://github.com/).
2. Klicke auf `Sign up`.
3. Erstelle einen Account mit deiner E-Mail-Adresse.
4. Bestätige deine E-Mail-Adresse.
5. Merke dir deinen Benutzernamen.

Du brauchst keinen bezahlten Plan.

### 2. Terminal öffnen

Das `Terminal` ist ein Programm, in dem du Textbefehle ausführst.

1. Drücke `Cmd + Leertaste`.
2. Tippe `Terminal`.
3. Drücke `Enter`.

Du siehst jetzt ein Fenster, in das du Befehle schreiben kannst.

### 3. Homebrew installieren

`Homebrew` installiert Programme auf deinem Mac.

Kopiere diesen Befehl in das Terminal und drücke `Enter`:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Der Installer erklärt, was er macht. Wenn er nach deinem Passwort fragt: Tippe dein Mac-Passwort ein und drücke `Enter`.

Wichtig: Beim Tippen des Passworts siehst du keine Zeichen. Das ist normal.

Wenn Homebrew am Ende Hinweise zu `Next steps` zeigt, führe diese Befehle ebenfalls aus. Danach schließe das Terminal und öffne es neu.

Prüfe danach:

```sh
brew --version
```

Wenn eine Versionsnummer erscheint, ist `Homebrew` installiert.

### 4. Git installieren

`Git` speichert Versionen deines Projekts. Dadurch kannst du später nachvollziehen, was sich geändert hat.

Installiere `Git`:

```sh
brew install git
```

Prüfe danach:

```sh
git --version
```

Wenn eine Versionsnummer erscheint, ist `Git` installiert.

### 5. Git einmal einrichten

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

### 6. Node.js LTS installieren

`Node.js` hilft uns später, einfache Webprojekte lokal auszuführen. `LTS` bedeutet: stabile Version für die meisten Nutzerinnen und Nutzer.

Installiere `Node.js`:

```sh
brew install node
```

Prüfe danach:

```sh
node --version
npm --version
```

Wenn beide Befehle eine Versionsnummer anzeigen, ist alles bereit.

### 7. Zed installieren

`Zed` ist unser Code Editor. Darin öffnest und bearbeitest du Projektdateien.

Installiere `Zed`:

```sh
brew install --cask zed
```

Starte danach `Zed` aus dem Programme-Ordner oder über Spotlight:

1. Drücke `Cmd + Leertaste`.
2. Tippe `Zed`.
3. Drücke `Enter`.

### 8. OpenCode installieren

`OpenCode` ist der Coding Agent, den wir im Workshop verwenden wollen. Er läuft im Terminal.

Installiere `OpenCode`:

```sh
brew install anomalyco/tap/opencode
```

Prüfe danach:

```sh
opencode --version
```

Wenn eine Versionsnummer erscheint, ist OpenCode installiert.

Falls das nicht funktioniert, nutze die `npm`-Variante:

```sh
npm install -g opencode-ai
```

### 9. OpenCode in Zed hinzufügen

OpenCode kann in Zed als `External Agent` laufen. Dann kannst du direkt in Zed mit dem Agenten chatten, während dein Projektordner geöffnet ist.

So fügst du OpenCode in Zed hinzu:

1. Öffne `Zed`.
2. Öffne dein Projekt oder den Ordner `erstes-projekt`.
3. Öffne die Command Palette mit `Cmd + Shift + P`.
4. Suche nach `zed: acp registry`.
5. Öffne die ACP Registry.
6. Suche nach `OpenCode`.
7. Installiere den OpenCode-Agenten.
8. Öffne das Agent Panel über das ✨-Symbol oder über die Command Palette mit `agent: new thread`.
9. Wähle im neuen Thread `OpenCode` als Agent aus.

Wenn OpenCode dich zur Anmeldung oder Verbindung auffordert, folge den Anweisungen.

OpenCode braucht Zugriff auf ein KI-Modell. Je nach Workshop-Stand kann das über einen OpenCode-Account, einen API-Key oder einen anderen Provider laufen.

Wenn du nach einem API-Key gefragt wirst und noch keinen hast, warte auf die Erklärung im Workshop.

Du musst hier nichts kaufen, bevor wir gemeinsam geklärt haben, welchen Zugang wir verwenden.

Hinweis: Wenn du zufällig schon für einen anderen Coding Agent bezahlst, zum Beispiel `Codex`, `Claude Code`, `Copilot` oder einen anderen Agenten in Zed, kannst du auch diesen benutzen. Für den gemeinsamen Workshop-Flow verwenden wir aber OpenCode.

### 10. OpenCode im Terminal testen

Falls die Zed-Verbindung noch nicht funktioniert, kannst du OpenCode auch direkt im Terminal testen:

1. Öffne das Terminal.
2. Starte OpenCode:

```sh
opencode
```

### 11. Projektordner anlegen

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

### 12. Projekt in Zed öffnen

Öffne `Zed`.

Dann:

1. Klicke auf `File`.
2. Klicke auf `Open Folder`.
3. Wähle den Ordner `erstes-projekt`.
4. Öffne ihn.

Du siehst jetzt deinen Projektordner in Zed. Er ist noch leer. Das ist normal.

---

## Kurzer Funktionstest

Gehe im Terminal in deinen Projektordner:

```sh
cd ~/Desktop/vibe-coding-projekte/erstes-projekt
```

Starte OpenCode:

```sh
opencode
```

Wenn OpenCode im Terminal startet oder als Agent in Zed auswählbar ist, bist du bereit für den Workshop.

Wenn OpenCode nicht startet, prüfe:

- Gibt `brew --version` eine Versionsnummer aus?
- Gibt `node --version` eine Versionsnummer aus?
- Gibt `npm --version` eine Versionsnummer aus?
- Gibt `opencode --version` eine Versionsnummer aus?
- Bist du im richtigen Ordner?

## Was du jetzt gelernt hast

Du hast deinen Mac so vorbereitet, dass du mit einem Coding Agent an einem eigenen Projekt arbeiten kannst.

Du hast außerdem gesehen, dass ein Projekt nicht mit Code beginnt, sondern mit einer einfachen Arbeitsumgebung: Account, Package Manager, Editor, Terminal, Projektordner und Agent.
