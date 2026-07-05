# Anleitungen 

## Webseite lokal ausführen

Virtuelle Umgebung anlegen:

```commandline
python -m venv venv
```

Virtuelle Umgebung aktivieren:

Auf Windows:

```commandline
.\venv\Scripts\Activate.ps1
```

Auf macOS oder Linux:

```commandline
source venv/bin/activate
```

Abhängigkeiten installieren:

```commandline
pip install -r requirements.txt
```

Lokal Webseite ausführen:

```commandline
mkdocs serve
```

## Webseite veröffentlichen (einmalig)

Gehe in Github auf ":octicons-gear-16: Settings".

Gehe auf ":octicons-browser-16: Pages".

Unter "Source" wähle "Deploy from branch" aus.

Unter "Branch" wähle "gh-pages" aus.

Die Webseite ist nach einigen Minuten online und erreichbar.

Wenn der Branch "gh-pages" noch nicht existiert, wird dieser automatisch erstellt, wenn zum ersten mal etwas auf den "main"-Branch gepusht wird (wegen der ci-Pipeline).

## Inhalte veröffentlichen

Um Inhalte zu veröffentlichen, pushe diese einfach inden "main"-Branch.

Die Änderungen sind nach ca. 30-50 Sekunden ausgerollt.
