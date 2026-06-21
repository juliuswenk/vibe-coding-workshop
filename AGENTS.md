# AGENTS.md

Dieses Repo enthält die studentische Website für den Vibe Coding Workshop an der SRH.
Alle Änderungen sollen darauf einzahlen, dass Studierende ohne Coding-, Git- oder Terminal-Erfahrung dem Workshop sicher folgen können.

## Website

- Die Website wird mit GitHub Pages gebaut.
- Standard ist `jekyll-theme-minimal`.
- Die zweispaltige Minimal-Theme-Struktur soll erhalten bleiben: Navigation/Meta links, Inhalt rechts.
- Keine eigene Frontend-App, kein React/Vite/Next, kein unnötiges JavaScript, solange Markdown und Jekyll reichen.
- Styling nur anfassen, wenn es ausdrücklich gewünscht ist oder die Lesbarkeit klar verbessert.
- Wenn Styling geändert wird, kleine Änderungen bevorzugen: Farben, Abstände, Typografie, Navigation.
- Die Website ersetzt Slides. Keine Slide-Struktur planen, außer sie wird ausdrücklich angefordert.

## Inhaltliche Zielgruppe

- Die Studierenden haben wahrscheinlich noch nie mit Git, GitHub, Terminal oder Code gearbeitet.
- Begriffe müssen langsam eingeführt werden.
- Jede Anleitung soll ohne Vorwissen verständlich sein.
- Keine vorausgesetzten Abkürzungen wie "Repo klonen", "Commit machen" oder "Dependency installieren", ohne sie kurz zu erklären.
- Vibe Coding soll als Werkzeug vermittelt werden, nicht als magische Komplettlösung.
- Wichtig ist: Konzepte, gutes Zerlegen von Problemen und iteratives Arbeiten mit Coding Agents.

## Sprache und Ton

- Studentische Inhalte sind überwiegend auf Deutsch.
- Etablierte englische Fachbegriffe bleiben auf Englisch, zum Beispiel `Prompt`, `Coding Agent`, `Repository`, `Commit`, `Branch`, `Markdown`, `Vibe Coding`.
- Beim ersten Auftauchen eines wichtigen Begriffs kurz erklären, was er praktisch bedeutet.
- Ton: klar, ruhig, anleitend und leicht ermutigend.
- Keine akademische Distanz, aber auch kein Marketing-Ton.
- Gelegentlich darauf hinweisen, was die Studierenden bereits geschafft haben.

## Seitenstruktur

- Eine Markdown-Datei pro Thema.
- Kurze, stabile Dateinamen in kebab-case verwenden.
- Seiten so schneiden, dass Studierende während des Workshops schnell die richtige Stelle finden.
- Lange Sammelseiten vermeiden, wenn mehrere eigenständige Schritte entstehen.
- Interne Links zwischen zusammengehörigen Seiten setzen.

Geplante Struktur:

```text
index.md
theorie.md
setup/
  mac.md
  windows.md
tutorials/
  github.md
  zed.md
  coding-agent.md
mein-erstes-projekt.md
freies-projekt-inspiration.md
glossar.md
knowledge-base.md
```

Die Struktur darf angepasst werden, wenn dadurch die Nutzung im Workshop einfacher wird.

## Pflichtstruktur Für Jede Inhaltsseite

Jede studentische `.md`-Datei soll diese drei Orientierungsteile enthalten:

1. Am Anfang: `## Was diese Seite erklärt`
   - Kurz sagen, worum es auf der Seite geht.
   - Maximal wenige Absätze oder eine kurze Liste.

2. Danach: `## Warum das für Vibe Coding wichtig ist`
   - Erklären, welchen Nutzen dieser Teil für das Arbeiten mit Coding Agents hat.
   - Praktisch bleiben: Was können Studierende danach besser entscheiden, vorbereiten oder ausführen?

3. Am Ende: `## Was du jetzt gelernt hast`
   - Kurz zusammenfassen, was die Studierenden nach diesem Abschnitt können oder verstanden haben.
   - Darf ermutigend sein, aber konkret bleiben.

Beispiel:

```md
## Was diese Seite erklärt

Diese Seite zeigt dir, wie du ...

## Warum das für Vibe Coding wichtig ist

Ein Coding Agent kann besser helfen, wenn ...

...

## Was du jetzt gelernt hast

Du hast jetzt ...
```

## Schreibregeln Für Anleitungen

- Schritte nummerieren, wenn sie in einer festen Reihenfolge passieren müssen.
- Kurze Absätze verwenden.
- Code, Dateinamen, Befehle und technische Begriffe in Backticks setzen.
- Keine langen Theorieblöcke ohne konkrete Anwendung.
- Bei Befehlen kurz sagen, wo sie ausgeführt werden.
- Fehlerstellen vorwegnehmen, wenn Anfänger dort wahrscheinlich hängen bleiben.
- Screenshots oder einfache Visualisierungen sind willkommen, wenn sie Studierenden wirklich helfen.
- Visuelle Würze ist erlaubt: kleine Diagramme, Icons, Screenshots, Skizzen oder einfache Callouts.
- Visuelle Elemente dürfen die Seite nicht schwerer wartbar machen.

## Workshop-Philosophie

- Einfachheit gewinnt.
- Markdown vor Custom Code.
- Vorhandene Jekyll-/GitHub-Pages-Funktionen vor eigener Logik.
- Keine Features "für später" bauen.
- Keine Tooling-Annahmen in `AGENTS.md` festschreiben, da sich die Workshop-Tools ändern können.
- Inhalte müssen während eines 4-Stunden-Workshops nutzbar sein: schnell auffindbar, klar gegliedert, nicht überladen.

## Was Nicht In Dieses Repo Gehört

- Komplexe Web-App-Strukturen.
- Unnötige Build-Tools.
- Ungefragte Design-Systeme.
- Lange Präsentationsfolien als Ersatz für die Website.
- Musterlösungen außerhalb des ausdrücklich vorgesehenen Bereichs.

## Prüfen Vor Abschluss

- Neue oder geänderte Seiten in der GitHub-Pages-Struktur verlinken.
- Prüfen, ob Anfänger die Begriffe verstehen können.
- Prüfen, ob jede Inhaltsseite die drei Pflichtteile enthält.
- Prüfen, ob die zweispaltige Minimal-Theme-Struktur erhalten bleibt.
- Bei größeren Seiten lokal bauen oder zumindest die Markdown-Struktur sorgfältig prüfen.
