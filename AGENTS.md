# X

X ist ein eigenständiges Holon für Beiträge auf der Plattform X und die spätere Verarbeitung ihrer Resonanz.

## Arbeitsmodell

- Sichtbare Dateien und Verzeichnisse enthalten Entwürfe, veröffentlichte Serien und technische Ausgaben.
- `.agents/` enthält Rollen, Prozesse, Lernprotokolle und Formatkonventionen.
- `AGENTS.md` ist der Einstiegspunkt und verweist auf die zuständige Rolle.

## Routing

| Signal oder Auftrag | Zuständige Rolle |
| --- | --- |
| Ein veröffentlichter Blogartikel soll vollständig verarbeitet werden | `.agents/roles/coordinator/AGENTS.md` |
| Ein ausdrücklicher Einzelauftrag an Autor, Editor oder Herausgeber | `.agents/roles/coordinator/AGENTS.md` |

Vor der Arbeit die verlinkte `AGENTS.md` vollständig lesen. Der Koordinator wählt den passenden eigenen Prozess und verweist auf die einzelnen Rollen.

## Grenzen

- Nur veröffentlichte Blogartikel als Quelle verwenden.
- Keine Plattform oder API anbinden.
- Keine Inhalte aus Knowledge übernehmen.
- Bestehende, nicht zur Aufgabe gehörende Änderungen bleiben unangetastet.
