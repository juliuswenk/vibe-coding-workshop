---
layout: default
title: Setup für Windows
---

# Setup für Windows

Diese Seite hilft dir dabei, deinen Windows-Computer für den Workshop vorzubereiten.

Wir nutzen `winget` als Package Manager. Ein Package Manager installiert Programme über Befehle in PowerShell. Das wirkt am Anfang ungewohnt, ist aber oft einfacher als viele einzelne Downloadseiten.

## Was diese Seite erklärt

Du installierst und prüfst:

- einen GitHub-Account
- `winget`
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

Öffne diese Seite auf deinem Windows-Computer und arbeite die Schritte von oben nach unten durch.

Wenn ein Schritt nicht funktioniert: Nicht schlimm. Schreib dir die Fehlermeldung auf oder mach einen Screenshot.

## 1. GitHub-Account erstellen

`GitHub` ist eine Website, auf der du Code speichern und teilen kannst. Für den Workshop brauchst du einen kostenlosen persönlichen Account.

1. Öffne [github.com](https://github.com/).
2. Klicke auf `Sign up`.
3. Erstelle einen Account mit deiner E-Mail-Adresse.
4. Bestätige deine E-Mail-Adresse.
5. Merke dir deinen Benutzernamen.

Du brauchst keinen bezahlten Plan.

## 2. PowerShell öffnen

`PowerShell` ist ein Programm, in dem du Textbefehle ausführst.

1. Drücke die `Windows`-Taste.
2. Tippe `PowerShell`.
3. Öffne `Windows PowerShell`.

Du siehst jetzt ein Fenster, in das du Befehle schreiben kannst.

## 3. winget prüfen

`winget` ist der Windows Package Manager. Auf Windows 11 und aktuellen Windows-10-Versionen ist er meistens schon installiert.

Prüfe in PowerShell:

```powershell
winget --version
```

Wenn eine Versionsnummer erscheint, ist `winget` bereit.

Wenn der Befehl nicht gefunden wird:

1. Öffne den `Microsoft Store`.
2. Suche nach `App Installer`.
3. Installiere oder aktualisiere `App Installer`.
4. Schließe PowerShell und öffne sie neu.
5. Prüfe nochmal:

```powershell
winget --version
```

## 4. Git installieren

`Git` speichert Versionen deines Projekts. Dadurch kannst du später nachvollziehen, was sich geändert hat.

Installiere `Git`:

```powershell
winget install --id Git.Git -e
```

Schließe PowerShell danach und öffne sie neu.

Prüfe dann:

```powershell
git --version
```

Wenn eine Versionsnummer erscheint, ist `Git` installiert.

## 5. Git einmal einrichten

Git soll wissen, welcher Name und welche E-Mail-Adresse zu deinen Änderungen gehören.

Ersetze die Beispielwerte durch deine Daten:

```powershell
git config --global user.name "Dein Name"
git config --global user.email "deine-mail@example.com"
```

Prüfe danach:

```powershell
git config --global user.name
git config --global user.email
```

Wenn dein Name und deine E-Mail-Adresse angezeigt werden, passt es.

## 6. Node.js LTS installieren

`Node.js` hilft uns später, einfache Webprojekte lokal auszuführen. `LTS` bedeutet: stabile Version für die meisten Nutzerinnen und Nutzer.

Installiere `Node.js LTS`:

```powershell
winget install --id OpenJS.NodeJS.LTS -e
```

Schließe PowerShell danach und öffne sie neu.

Prüfe die Installation:

```powershell
node --version
npm --version
```

Wenn beide Befehle eine Versionsnummer anzeigen, ist alles bereit.

## 7. Zed installieren

`Zed` ist unser Code Editor. Darin öffnest und bearbeitest du Projektdateien.

Prüfe zuerst, ob Zed über `winget` verfügbar ist:

```powershell
winget search Zed
```

Wenn du einen Eintrag für `Zed` siehst, installiere ihn. Meistens ist der Paketname:

```powershell
winget install --id Zed.Zed -e
```

Wenn `winget` keinen Zed-Eintrag findet, nutze die offizielle Downloadseite:

1. Öffne [zed.dev/download](https://zed.dev/download).
2. Lade Zed für Windows herunter.
3. Starte den Installer.
4. Öffne danach `Zed`.

## 8. OpenCode installieren

`OpenCode` ist der Coding Agent, den wir im Workshop verwenden wollen. Er läuft in PowerShell.

Installiere OpenCode mit `npm`:

```powershell
npm install -g opencode-ai
```

Prüfe danach:

```powershell
opencode --version
```

Wenn eine Versionsnummer erscheint, ist OpenCode installiert.

## 9. OpenCode verbinden

OpenCode braucht Zugriff auf ein KI-Modell. Je nach Workshop-Stand kann das über einen OpenCode-Account, einen API-Key oder einen anderen Provider laufen.

Für jetzt reicht:

1. Öffne PowerShell.
2. Starte OpenCode:

```powershell
opencode
```

3. Wenn OpenCode dich zur Anmeldung oder Verbindung auffordert, folge den Anweisungen.
4. Wenn du nach einem API-Key gefragt wirst und noch keinen hast, warte auf die Erklärung im Workshop.

Du musst hier nichts kaufen, bevor wir gemeinsam geklärt haben, welchen Zugang wir verwenden.

## 10. Projektordner anlegen

Ein Projektordner ist einfach ein Ordner, in dem alle Dateien deines Projekts liegen.

Lege auf dem Desktop einen Ordner an:

```powershell
cd Desktop
mkdir vibe-coding-projekte
cd vibe-coding-projekte
mkdir erstes-projekt
cd erstes-projekt
```

Prüfe, wo du bist:

```powershell
pwd
```

Du solltest einen Pfad sehen, der ungefähr so endet:

```text
Desktop\vibe-coding-projekte\erstes-projekt
```

## 11. Projekt in Zed öffnen

Öffne `Zed`.

Dann:

1. Klicke auf `File`.
2. Klicke auf `Open Folder`.
3. Wähle den Ordner `erstes-projekt`.
4. Öffne ihn.

Du siehst jetzt deinen Projektordner in Zed. Er ist noch leer. Das ist normal.

## 12. Kurzer Funktionstest

Gehe in PowerShell in deinen Projektordner:

```powershell
cd Desktop\vibe-coding-projekte\erstes-projekt
```

Starte OpenCode:

```powershell
opencode
```

Wenn OpenCode startet, bist du bereit für den Workshop.

Wenn OpenCode nicht startet, prüfe:

- Gibt `winget --version` eine Versionsnummer aus?
- Gibt `node --version` eine Versionsnummer aus?
- Gibt `npm --version` eine Versionsnummer aus?
- Gibt `opencode --version` eine Versionsnummer aus?
- Bist du im richtigen Ordner?

## Was du jetzt gelernt hast

Du hast deinen Windows-Computer so vorbereitet, dass du mit einem Coding Agent an einem eigenen Projekt arbeiten kannst.

Du hast außerdem gesehen, dass ein Projekt nicht mit Code beginnt, sondern mit einer einfachen Arbeitsumgebung: Account, Package Manager, Editor, PowerShell, Projektordner und Agent.
