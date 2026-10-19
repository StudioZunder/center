# Auftrag für Claude Code: Bruns Timer auf GitHub

## Projekt
Statischer Timer im Bruns-Design. Alles steckt in `index.html`.
Kein Build, kein Framework, keine Abhängigkeiten außer Google Fonts.

## Aufgabe
1. Prüfe, ob `git` und `gh` installiert sind und `gh auth status` angemeldet ist.
   Falls nicht: Nutzer bitten, `gh auth login` auszuführen.
2. Git-Repo initialisieren, Branch `main`.
3. Ersten Commit erstellen: „Bruns Timer 60: erste Version“.
4. Öffentliches Repo anlegen und pushen:
   `gh repo create bruns-timer --public --source=. --remote=origin --push`
5. GitHub Pages aktivieren (Branch `main`, Ordner `/`):
   `gh api -X POST repos/{owner}/bruns-timer/pages -f "source[branch]=main" -f "source[path]=/"`
6. Am Ende die Pages-Adresse ausgeben: `https://<owner>.github.io/bruns-timer/`

## Regeln für spätere Änderungen
- Design: Bruns-Look nach Dieter Rams. Warmes Hellgrau, schwarzes Zifferblatt,
  gelber Zeiger, orange Start-Taste, graue Reset-Taste. Schrift Archivo.
- Farben nur über die Tokens im `:root`-Block ändern.
- Alles bleibt in einer Datei. Keine Bibliotheken hinzufügen.
- Texte auf Deutsch. Kurze Sätze. Keine Gedankenstriche, keine Emoticons.
- Nach jeder Änderung committen und pushen.
