# Thread-Exporte

Eine Datei repräsentiert genau einen Thread aus einem Ursprungsgespräch. Dateiname: stabiler Gegenstandsname mit `.json`. Das Array `posts` steht in verbindlicher Lesereihenfolge; seine Elemente sind Teile desselben Threads, keine unabhängigen Veröffentlichungen.

```json
{
  "schema_version": 1,
  "title": "Titel des Denkwegs",
  "source": {
    "conversation": "Eindeutige Gesprächsreferenz",
    "article": "../blog/Quelldatei.md"
  },
  "posts": [
    {"message": "Konkrete Beobachtung und eingelöster Hook."},
    {"message": "Eine eigenständige Erkenntnis oder echte offene Frage als Abschluss."}
  ]
}
```

`source.article_url` ist optional und wird ohne bestätigte öffentliche Artikel-URL weggelassen. Kein Platzhalter und keine Repository-URL als Ersatz. Ein fehlender Link blockiert den Export nicht.

`title` ist interne Orientierung; der erste `message` ist der veröffentlichte Einstieg. Keine Zeitstempel, Termine oder Buffer-Felder. d15r.de übernimmt Import, Planung und Versand. Dieses neue Format ist der Exportvertrag des X-Holons; die Unterstützung durch den d15r.de-Importer ist nicht durch diesen Prozess belegt. Keine automatische Konvertierung alter `posts/`-Serien.

Schema: `schema.json`. Zusätzlich redaktionell und technisch prüfen: gewichtete X-Zeichenlänge jedes Beitrags, eigenständiger Abschluss, gegebenenfalls bestätigter optionaler Link, Quellenreferenzen und unveränderte Reihenfolge des freigegebenen Entwurfs. Diese Anforderungen werden nicht vollständig durch JSON Schema abgedeckt.
