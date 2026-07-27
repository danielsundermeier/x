# X

X ist ein eigenständiges Repository-Holon für Beiträge auf der Plattform X und die spätere Verarbeitung ihrer Resonanz.

## Rollen

X besteht aus drei Rollen-Holons:

1. `holons/autor/` entwickelt oder überarbeitet X-Beiträge aus einem veröffentlichten Blogartikel.
2. `holons/editor/` bewertet die Beiträge und gibt strukturiertes Feedback.
3. `holons/herausgeber/` terminiert freigegebene Beiträge, erzeugt die JSON-Ausgabe und veröffentlicht sie im X-Repository.

## Standardworkflow

Bei einem Auftrag, X-Beiträge aus einem veröffentlichten Blogartikel zu erstellen:

1. Autor erstellt einen Entwurf unter `drafts/`.
2. Editor bewertet den Entwurf.
3. Autor und Editor wiederholen ihre Schritte bei Bedarf, höchstens bis Iteration 3.
4. Bei `status: freigabe` oder `status: abgeschlossen` übernimmt der Herausgeber automatisch.
5. Bei `status: blockiert` endet der Ablauf in `drafts/` und der Grund wird gemeldet.

Der Standardworkflow endet erst nach Archivierung, JSON-Ausgabe, Commit und Push durch den Herausgeber oder mit einem blockierten Entwurf.

## Einzelne Rollen aufrufen

Jede Rolle kann ausnahmsweise einzeln beauftragt werden:

- `Autor`: erstellt oder überarbeitet nur einen Entwurf und stoppt.
- `Editor`: bewertet nur den genannten Entwurf und stoppt.
- `Herausgeber`: verarbeitet nur den genannten freigegebenen oder abgeschlossenen Entwurf.

Bei einem Einzelauftrag keine vorherige oder nachfolgende Rolle automatisch starten.

## Grenzen

- Nur veröffentlichte Blogartikel als Quelle verwenden.
- Keine Plattform oder API anbinden.
- Keine Inhalte aus Knowledge übernehmen.
- Autor und Editor erstellen keine Commits oder Pushes.
- Der Herausgeber committed und pusht ausschließlich die von ihm veröffentlichte X-Serie.
- Bestehende, nicht zur Aufgabe gehörende Änderungen bleiben unangetastet.
