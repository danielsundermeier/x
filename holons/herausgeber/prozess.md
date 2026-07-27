# Prozess des Herausgebers

## 1. Entwurf prüfen

- Der Workflow übergibt genau eine Datei unter `drafts/`.
- Das Frontmatter ist gültig.
- `status` ist `freigabe` oder `abgeschlossen`.
- `anzahl` entspricht der tatsächlichen Zahl nummerierter Beiträge.
- Jeder Beitrag erfüllt die aktuelle Zeichenbegrenzung der Plattform.

Wenn eine Bedingung nicht erfüllt ist, nicht veröffentlichen und den Grund melden.

## 2. Frühesten möglichen Start bestimmen

- Das heutige lokale Datum in `Europe/Berlin` bestimmen.
- Das Veröffentlichungsdatum aus dem Dateinamen des Quellartikels bestimmen.
- Das spätere dieser beiden Daten als frühestmöglichen Start verwenden.
- Alle Datumswerte in vorhandenen JSON-Dateien unter `posts/` sammeln.

## 3. Beiträge terminieren

- Für den ersten Beitrag am frühestmöglichen Start beginnen.
- Ist ein Tag bereits belegt, jeweils einen Kalendertag weitergehen.
- Jedem folgenden Beitrag den nächsten freien Tag zuweisen.
- Höchstens einen Beitrag pro Tag planen.
- Keine künstlichen Pausen einfügen.

## 4. JSON erzeugen

Unter `posts/<ARTIKELNAME>.json` ein valides JSON-Array erzeugen:

```json
[
  {
    "date": "YYYY-MM-DD",
    "message": "Text des Beitrags"
  }
]
```

- Reihenfolge des geprüften Entwurfs beibehalten.
- Nur `date` und `message` ausgeben.
- Keine Markdown-Überschriften übernehmen.
- JSON syntaktisch validieren.

## 5. Entwurf archivieren

- Im Frontmatter `status: veroeffentlicht` setzen.
- Den ersten und letzten vergebenen Tag unter `veroeffentlichung.von` und `veroeffentlichung.bis` ergänzen.
- Den Entwurf aus `drafts/` nach `published/` verschieben.
- Inhalt und Editorbewertung nicht verändern.

## 6. Committen

- Vor dem Staging den Git-Status prüfen.
- Ausschließlich die neue JSON-Datei sowie den archivierten Entwurf und gegebenenfalls dessen versionierte Verschiebung stagen.
- Keine anderen Dateien aufnehmen.
- Den Titel des Quellartikels als Commit-Betreff verwenden.

Commit-Format:

```text
<Titel des Quellartikels>

X-Serie mit <ANZAHL> Beiträgen vom <VON> bis <BIS> veröffentlicht.
```

## 7. Pushen

- Den aktuellen Branch zum konfigurierten Upstream pushen.
- Niemals Force-Push verwenden.
- Bei einem Fehler stoppen und den Fehler melden.

## 8. Ergebnis melden

- JSON-Pfad und Archivpfad nennen.
- Anzahl und Zeitraum nennen.
- Commit-ID und gepushten Branch nennen.
- Bestätigen, dass keine unabhängigen Änderungen committed wurden.
