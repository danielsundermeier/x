# X

X ist ein eigenständiges Holon für Beiträge auf der Plattform X und die spätere Verarbeitung ihrer Resonanz.

Die kanonische Identität des medienübergreifenden Creators lebt unter
`../d15r/.agents/roles/creator/soul/AGENTS.md`. X-Rollen lesen sie als
gemeinsamen Identitätskontext und entwickeln daraus ihre eigene kurze Form.

## Arbeitsmodell

- Sichtbare Dateien und Verzeichnisse enthalten Entwürfe, veröffentlichte Serien und technische Ausgaben.
- `.agents/` enthält Rollen, Prozesse, gegenstandsbezogene Lerndateien und
  Formatkonventionen.
- `AGENTS.md` ist der Einstiegspunkt und verweist auf die zuständige Rolle.

Jeder Agent gestaltet seinen eigenen Arbeitsbereich und entwickelt ihn nach jedem Zyklus weiter. Dafür gilt `.agents/conventions/evolution.md`.

## Neuer Standard

Für die Gesprächsverarbeitung gilt ein Thread pro Ursprungsgespräch mit zugehörigem veröffentlichtem Blogartikel. Import, Planung und Versand übernimmt d15r.de.

## Routing

| Signal oder Auftrag | Zuständige Rolle |
| --- | --- |
| Ein Gespräch mit zugehörigem veröffentlichtem Blogartikel soll als Thread verarbeitet werden | `.agents/roles/coordinator/AGENTS.md` |
| Ein veröffentlichter Blogartikel soll vollständig verarbeitet werden | `.agents/roles/coordinator/AGENTS.md` |
| Ein ausdrücklicher Einzelauftrag an Autor, Editor oder Herausgeber | `.agents/roles/coordinator/AGENTS.md` |
| Liegengebliebene X-Arbeitsgegenstände sollen nachgeholt oder fortgesetzt werden | `.agents/roles/coordinator/AGENTS.md` |

Vor der Arbeit die verlinkte `AGENTS.md` vollständig lesen. Der Koordinator wählt den passenden eigenen Prozess und verweist auf die einzelnen Rollen.

## Grenzen

- Im Thread-Prozess das vollständige Ursprungsgespräch und den zugehörigen veröffentlichten Blogartikel als Quellen verwenden; im historischen Artikelprozess nur veröffentlichte Blogartikel.
- Keine Plattform oder API anbinden.
- Keine Inhalte aus Knowledge übernehmen.
- Keine direkten Änderungen an d15r oder seiner Soul vornehmen.
- Beobachtungen über den Creator nur an dessen zuständige Rolle zurückgeben.
- Bestehende, nicht zur Aufgabe gehörende Änderungen bleiben unangetastet.
