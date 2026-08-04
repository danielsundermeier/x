# Liegengebliebene X-Arbeitsgegenstände nachholen

## Eingang

Ein Auftrag verlangt, vorhandene, noch nicht fertig verarbeitete
Arbeitsgegenstände des X-Holons nachzuholen oder fortzusetzen.

## Ablauf

1. Die sichtbaren Arbeitsgegenstände unter `drafts/`, `published/` und `posts/`
   inventarisieren. README-Dateien und technische Hilfsdateien sind keine
   Arbeitsgegenstände.
2. Für jeden noch nicht fertig verarbeiteten Gegenstand den nächsten Schritt
   ausschließlich aus seinem dokumentierten Zustand bestimmen:
   - `status: entwurf` → Editor
   - `status: ueberarbeitung` → Autor
   - `status: freigabe` oder `status: abgeschlossen` → Herausgeber
   - `status: veroeffentlicht` mit vorhandener Markdown- und JSON-Ausgabe →
     fertig, keine Rolle aufrufen
   - `status: blockiert`, ein fehlender oder unbekannter Status oder
     widersprüchliche Ausgaben → nicht raten, sondern als Blocker melden
3. Nur für tatsächlich zu übergebende Arbeitsgegenstände die `AGENTS.md` der
   jeweils zuständigen Rolle vollständig lesen:
   - `../autor/AGENTS.md`
   - `../editor/AGENTS.md`
   - `../herausgeber/AGENTS.md`
4. Jede zuständige Rolle mit den ihr zugeordneten Arbeitsgegenständen
   auffordern, ihren bestehenden Prozess selbst auszuführen.
5. Nach jedem Rollenlauf den neuen dokumentierten Zustand erneut prüfen.
   Folgezustände erneut nach Schritt 2 übergeben, bis jeder Gegenstand fertig
   oder eindeutig blockiert ist.
6. Übergaben, abgeschlossene Gegenstände und Blocker melden.
7. Den Koordinator-Durchgang nach `../../conventions/evolution.md` auswerten
   und nur relevante neue Erfahrung gegenstandsbezogen unter `lernen/`
   festhalten.

## Grenzen

- Der Koordinator verändert keine Inhalte, Bewertungen, Termine oder
  technischen Ausgaben.
- Er führt keinen Rollenprozess stellvertretend aus und verändert keinen
  Rollenprozess.
- Er leitet nur Zustände weiter, die an den Arbeitsgegenständen tatsächlich
  dokumentiert sind.
- Er sucht nicht außerhalb des X-Holons nach mutmaßlich fehlenden
  Arbeitsgegenständen.
- Bestehende, nicht zum Nachholauftrag gehörende Änderungen bleiben
  unangetastet.
- Commit und Push führt der Koordinator nicht selbst aus.
