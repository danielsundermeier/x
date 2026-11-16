# Ein Thread pro Gespräch

## Ziel und Quellen

Pro verarbeitetem Gespräch entsteht genau ein zusammenhängender Thread. Er soll Menschen anziehen, die an den konkreten Fragen, Beobachtungen und Verbindungen des Creators interessiert sind. Reichweite, Klicks und Beitragsmenge sind keine Qualitätsziele.

Hauptquelle ist das vollständige Ursprungsgespräch; der zugehörige veröffentlichte Blogartikel liefert das Ergebnis als Kontext. Eine öffentliche Artikel-URL ist keine Voraussetzung. Gedanken aus dem Gespräch dürfen verwendet werden, auch wenn sie im Artikel fehlen. Vorschläge des Assistenten dürfen nicht als persönliche Erlebnisse oder Überzeugungen des Creators ausgegeben werden. Keine erfundenen Ereignisse, Übergänge oder nachträglich behaupteten Erkenntnisse.

## Autor

Gespräch, Artikel und gemeinsame Creator-Identität vollständig lesen. Einen interessanten Denkweg auswählen: konkrete Ausgangsbeobachtung, Assoziationen, überraschende Verbindungen, Zweifel oder Wendepunkt und eine tragfähige Erkenntnis. Auswahl und Verdichtung sind erlaubt; ein lückenloses Gesprächsprotokoll ist nicht das Ziel. Verbindungen erklären, statt lediglich Themen aufzuzählen. Nicht alle Gespräche in dieselbe Dramaturgie pressen.

Der erste Beitrag ist ein präziser Hook, dessen Versprechen der Thread einlöst. Keine künstliche Sensation oder zurückgehaltene Auflösung bis zum Blogklick. Der Thread muss ohne Artikel einen nachvollziehbaren, wertvollen Gedanken vermitteln. Jeder weitere Beitrag trägt etwas Neues bei und darf auf Vorheriges aufbauen. Konkrete Beobachtungen und verständliche Beispiele tragen abstrakte Verbindungen. Persönlich, klar, warm, neugierig und offen schreiben; keine allgemeine Lebensberatung oder Engagement-Köder.

Die Länge folgt der Substanz. Ein Thread umfasst mindestens zwei Beiträge; keine feste Zielzahl, keine Füllbeiträge. Pro Beitrag höchstens 280 nach X-Regeln gewichtete Zeichen einschließlich Links und eventueller Nummerierung; nicht bloß Python-Zeichen zählen. Den Thread mit einer eigenen Erkenntnis oder einer echten offenen Frage abschließen. Vorerst keinen Artikellink verlangen und keinen zusätzlichen Werbebeitrag anhängen. Nur wenn eine bestätigte öffentliche Artikel-URL vorliegt und ein Link gewünscht ist, darf der letzte Beitrag natürlich zum Artikel überleiten. Keine Artikeladresse erfinden oder eine Repository-URL als Ersatz einsetzen.

## Entwurf und Editor

Thread-Entwürfe liegen unter `drafts/threads/<gegenstand>.md`. Das bestehende Entwurfsfrontmatter wird um `format: thread`, `gespraech` (eindeutige Quellenreferenz) ergänzt; `artikel_url` ist optional und wird ohne bestätigte öffentliche URL weggelassen; `quelle` verweist weiterhin auf den Blogartikel. `anzahl` zählt die Beiträge dieses einen Threads. Das Thread-Format ersetzt hier die bisherige Vorgabe, jeden Beitrag allein aus dem Artikel abzuleiten und isoliert verständlich zu machen.

Der Autor begründet unter `strategie.ziel`, welcher Denkweg sichtbar wird und woran passende Menschen anknüpfen können. Bewertungsfelder bleiben dem Editor vorbehalten.

Der Editor liest beide Quellen und prüft: Löst der Hook sein Versprechen ein? Sind Verbindungen verständlich und quellentreu? Entsteht im Thread ein eigener Erkenntniswert? Bleiben Eigenheiten und Unsicherheiten erhalten? Gibt es Wiederholungen, künstliche Spannung oder bloße Werbung? Könnte ein interessierter Mensch mit einer eigenen Beobachtung oder einem begründeten Widerspruch anknüpfen? Stimmen Perspektive, Reihenfolge, Zeichenlimits und eigenständiger Abschluss? Einen optionalen Link nur prüfen, wenn er tatsächlich enthalten ist.

Bestehende Statuswerte und höchstens drei Autor-Iterationen gelten weiter. Nach der dritten Iteration bei wesentlichen Mängeln blockieren; Qualität nicht zur Erfüllung einer Quote absenken. Fehlendes Gespräch oder fehlender veröffentlichter Artikel sind konkrete Blocker. Eine fehlende öffentliche Artikel-URL blockiert weder Erstellung noch Freigabe oder Export.

## Herausgeber und Export

Nur freigegebene oder abgeschlossene Entwürfe exportieren. Inhalt und Reihenfolge unverändert übernehmen. Genau eine UTF-8-JSON-Datei unter `threads/<gegenstand>.json` erzeugen, gemäß `threads/README.md` und `threads/schema.json`. JSON syntaktisch und gegen das Schema prüfen; Übereinstimmung mit dem freigegebenen Entwurf, Quellen, Reihenfolge, Beitragszahl und Abschluss zusätzlich prüfen; einen optional enthaltenen Link gegen die bestätigte öffentliche URL prüfen. Geprüften Entwurf unter `published/threads/` archivieren und Exportstatus dokumentieren.

Keine Termine, Wochenquoten, Buffer-Aufrufe oder Veröffentlichung auf X. Import, Planung und Versand übernimmt ausschließlich d15r.de. Export ist keine Plattformveröffentlichung. Der Herausgeber darf nur auftragsbezogene Änderungen nach seinen bestehenden Regeln committen und ohne Force-Push pushen. Bestehende Serien und Dateien unter `posts/` bleiben erhalten.

Die Rollen werten nach ihrem Schritt jeweils nur den eigenen Bereich nach der Evolutionskonvention aus. Wirkung auf passende Kontakte erst anhand tatsächlicher Rückmeldungen beurteilen.
