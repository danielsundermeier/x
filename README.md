# X

X entwickelt aus veröffentlichten Blogartikeln Beiträge für die Plattform X.

## Rollen

```text
Blogartikel
    ↓
Autor
    ↓
Editor
    ↓
Herausgeber
```

Alle drei Rollen sind aktiv. Autor und Editor arbeiten in höchstens drei Iterationen; der Herausgeber terminiert und veröffentlicht eine freigegebene Serie im Repository.

## Struktur

- `AGENTS.md`: Routing und Grenzen des Repository-Holons
- `holons/autor/`: aktiver Erstellungsprozess
- `holons/editor/`: Bewertung und Feedback
- `holons/herausgeber/`: Terminierung, JSON-Ausgabe, Commit und Push
- `format/entwurf.md`: gemeinsames Entwurfsformat
- `drafts/`: noch nicht bewertete Beitragsserien
- `published/`: geprüfte Markdown-Entwürfe und ihre Prozessdaten
- `posts/`: terminierte JSON-Dateien für die technische Weiterverarbeitung

## Terminierung

Der erste Beitrag einer Serie erscheint am Datum des Quellartikels. Danach folgt innerhalb der Serie täglich ein weiterer Beitrag. Mehrere Beiträge aus unterschiedlichen Serien dürfen für denselben Tag geplant sein.
