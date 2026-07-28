# Format eines X-Entwurfs

Jeder Entwurf beschreibt eine aus einem Blogartikel entwickelte Gruppe von X-Beiträgen.

```yaml
---
quelle: "../blog/YYYY-MM-DD Titel.md"
beschreibung: ""
strategie:
  ziel: ""
  bewertung: ""
anzahl: 0
was_ist_gut: []
was_kann_ueberarbeitet_werden: []
ton:
  ziel: ""
  bewertung: ""
status: entwurf
iteration: 1
---
```

Danach folgen die Beiträge:

```markdown
# Titel des Quellartikels

## Beitrag 1

Text

## Beitrag 2

Text
```

## Verantwortung des Autors

- `quelle`
- `beschreibung`
- `strategie.ziel`
- `anzahl`
- `ton.ziel`
- `status`
- `iteration`
- Text der Beiträge

Die Bewertungsfelder bleiben zunächst leer. Sie werden später vom Editor gepflegt.

Der Editor setzt:

- `was_ist_gut`
- `was_kann_ueberarbeitet_werden`
- `strategie.bewertung`
- `ton.bewertung`
- `status`

## Regeln

- `quelle` verweist auf genau einen veröffentlichten Blogartikel.
- `anzahl` entspricht der tatsächlichen Zahl der Beiträge.
- Jeder Beitrag steht in einem eigenen nummerierten Abschnitt.
- Ein Entwurf enthält nur substanzielle Beiträge; es gibt keine feste Mindest- oder Höchstzahl.
- `iteration` darf höchstens den Wert `3` erreichen.
- Statuswerte sind `entwurf`, `ueberarbeitung`, `freigabe`, `abgeschlossen`, `blockiert` und `veroeffentlicht`.
- Nur `freigabe` und `abgeschlossen` dürfen an den Herausgeber übergeben werden.
