# X

## Standard für neue Gesprächsverarbeitungen

Ein Ursprungsgespräch und sein veröffentlichter Blogartikel werden zu genau einem eigenständigen Thread verarbeitet: Autor → Editor → Herausgeber → `threads/<gegenstand>.json`. Ziel sind passende Gesprächspartner durch nachvollziehbare Denkwege und eigenen Erkenntniswert. Der Thread endet eigenständig; eine öffentliche Artikel-URL ist optional und wird vorerst nicht benötigt. d15r.de übernimmt Import, Terminierung und Versand. Format und Schema stehen unter `threads/`; der Prozess unter `.agents/roles/coordinator/process-conversation.md`.

## Historische Artikelserien

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
- `.agents/roles/coordinator/`: Übergaben innerhalb des X-Holons
- `.agents/roles/autor/`: aktiver Erstellungsprozess
- `.agents/roles/editor/`: Bewertung und Feedback
- `.agents/roles/herausgeber/`: Terminierung, JSON-Ausgabe, Commit und Push
- `.agents/conventions/entwurf.md`: gemeinsames Entwurfsformat
- `drafts/`: noch nicht bewertete Beitragsserien
- `published/`: geprüfte Markdown-Entwürfe und ihre Prozessdaten
- `posts/`: terminierte JSON-Dateien für die technische Weiterverarbeitung

## Terminierung

Der erste Beitrag einer Serie erscheint am Datum des Quellartikels. Danach folgt innerhalb der Serie täglich ein weiterer Beitrag. Mehrere Beiträge aus unterschiedlichen Serien dürfen für denselben Tag geplant sein.
