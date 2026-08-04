# Prozess des Herausgebers

## 1. Entwurf prüfen

- Der Workflow übergibt genau eine Datei unter `drafts/`.
- Das Frontmatter ist gültig.
- `status` ist `freigabe` oder `abgeschlossen`.
- `anzahl` entspricht der tatsächlichen Zahl nummerierter Beiträge.
- Jeder Beitrag erfüllt die aktuelle Zeichenbegrenzung der Plattform.

Wenn eine Bedingung nicht erfüllt ist, nicht veröffentlichen und den Grund melden.

## 2. Startdatum bestimmen

- Das Veröffentlichungsdatum aus dem Dateinamen des Quellartikels bestimmen.
- Dieses Artikeldatum unverändert als Datum des ersten Beitrags verwenden.
- Bereits vorhandene Beiträge am selben Tag verändern oder verschieben dieses Datum nicht.

## 3. Beiträge terminieren

- Den ersten Beitrag auf das Artikeldatum legen.
- Jeden folgenden Beitrag dieser Serie genau einen Kalendertag später planen.
- Innerhalb dieser Serie höchstens einen Beitrag pro Tag planen.
- Beiträge aus anderen Serien dürfen dasselbe Datum haben.
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

## 6. Änderungen des Zyklus ermitteln

- Vor dem Staging den Git-Status prüfen.
- Die neue JSON-Datei sowie den archivierten Entwurf und gegebenenfalls dessen versionierte Verschiebung aufnehmen.
- Zusätzlich alle `prozess.md`- und gegenstandsbezogenen Dateien unter
  `lernen/` aufnehmen, die eine Rolle nachweislich während dieses X-Zyklus
  verändert hat.
- Weitere Dateien dürfen nur aufgenommen werden, wenn ihre Änderung unmittelbar aus diesem Zyklus stammt und für dessen Prozess erforderlich ist.
- Vorhandene Änderungen, deren Herkunft nicht eindeutig diesem Zyklus zugeordnet werden kann, nicht aufnehmen.
- Jede aufzunehmende Datei einzeln stagen; niemals pauschal das gesamte Repository stagen.

## 7. Committen

- Den Titel des Quellartikels als Commit-Betreff verwenden.

Commit-Format:

```text
<Titel des Quellartikels>

X-Serie mit <ANZAHL> Beiträgen vom <VON> bis <BIS> veröffentlicht.
Prozess verbessert: <kurze Beschreibung oder "keine Änderung">.
```

## 8. Pushen

- Den aktuellen Branch zum konfigurierten Upstream pushen.
- Niemals Force-Push verwenden.
- Bei einem Fehler stoppen und den Fehler melden.

## 9. Ergebnis melden

- JSON-Pfad und Archivpfad nennen.
- Anzahl und Zeitraum nennen.
- Commit-ID und gepushten Branch nennen.
- Die mitgeführten Prozess- und Lerndateien nennen.
- Bestätigen, dass keine unabhängigen Änderungen committed wurden.
