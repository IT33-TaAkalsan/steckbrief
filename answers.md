# Antworten

1) **Working Directory / Staging / Repository**
- Working Directory: Deine echten Dateien im Projektordner.
- Staging Area (Index): Zwischenbereich – was im nächsten Commit landet.
- Repository: Die Historie der Commits im `.git`-Ordner.

2) **Fast-Forward erkennen**
- `git merge --ff-only` läuft ohne Merge-Commit.
- `git log --oneline --graph` zeigt keinen Merge-Knoten; `main`-Zeiger rückt nur vor.

3) **Warum kann `--ff-only` fehlschlagen?**
- Wenn `main` seit dem Abzweigen eigene Commits hat → kein gerades Vorspulen mehr möglich.

4) **Vorteil von `dev`**
- Saubere Trennung von Arbeit und stabilem `main`, leichteres Review, weniger Risiko.

5) **Aktuellen Branch anzeigen**
- `git branch --show-current` (oder `git status`).

6) **Änderungen sichtbar & dauerhaft machen**
- Staging: `git add <datei>` (oder `git add .`)
- Commit: `git commit -m "Nachricht"`
