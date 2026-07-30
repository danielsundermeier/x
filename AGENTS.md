# X

X ist ein eigenständiges Holon für Beiträge auf der Plattform X und die spätere Verarbeitung ihrer Resonanz.

Die kanonische Identität des medienübergreifenden Creators lebt unter
`../d15r/.agents/roles/creator/soul/AGENTS.md`. X-Rollen lesen sie als
gemeinsamen Identitätskontext und entwickeln daraus ihre eigene kurze Form.

## Arbeitsmodell

- Sichtbare Dateien und Verzeichnisse enthalten Entwürfe, veröffentlichte Serien und technische Ausgaben.
- `.agents/` enthält Rollen, Prozesse, Lernprotokolle und Formatkonventionen.
- `AGENTS.md` ist der Einstiegspunkt und verweist auf die zuständige Rolle.

Jeder Agent gestaltet seinen eigenen Arbeitsbereich und entwickelt ihn nach jedem Zyklus weiter. Dafür gilt `.agents/conventions/evolution.md`.

## Routing

| Signal oder Auftrag | Zuständige Rolle |
| --- | --- |
| Ein veröffentlichter Blogartikel soll vollständig verarbeitet werden | `.agents/roles/coordinator/AGENTS.md` |
| Ein ausdrücklicher Einzelauftrag an Autor, Editor oder Herausgeber | `.agents/roles/coordinator/AGENTS.md` |
| Liegengebliebene X-Arbeitsgegenstände sollen nachgeholt oder fortgesetzt werden | `.agents/roles/coordinator/AGENTS.md` |

Vor der Arbeit die verlinkte `AGENTS.md` vollständig lesen. Der Koordinator wählt den passenden eigenen Prozess und verweist auf die einzelnen Rollen.

## Grenzen

- Nur veröffentlichte Blogartikel als Quelle verwenden.
- Keine Plattform oder API anbinden.
- Keine Inhalte aus Knowledge übernehmen.
- Keine direkten Änderungen an d15r oder seiner Soul vornehmen.
- Beobachtungen über den Creator nur an dessen zuständige Rolle zurückgeben.
- Bestehende, nicht zur Aufgabe gehörende Änderungen bleiben unangetastet.
