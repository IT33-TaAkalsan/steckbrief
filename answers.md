# Antworten zu den Kontrollfragen

1. **Unterschied Working Directory, Staging Area und Repository**
   - **Working Directory**: Dein Projektordner, in dem du Dateien bearbeitest.
   - **Staging Area (Index)**: Zwischenspeicher; hier legst du fest, welche Änderungen in den nächsten Commit aufgenommen werden.
   - **Repository**: Die Git-Datenbank im `.git`-Ordner, wo alle Commits und Versionen gespeichert sind.

2. **Woran erkennst du, ob ein Merge Fast-Forward war?**
   - Kein eigener Merge-Commit wird erstellt.
   - Der Branch-Zeiger springt nur nach vorne.
   - Im Log (`git log --oneline --graph`) sieht man eine gerade Linie ohne Verzweigung.

3. **Warum kann `git merge --ff-only` fehlschlagen?**
   - Wenn der Zielbranch (`main`) seit dem Abzweigen eigene Commits bekommen hat.

4. **Vorteil, Änderungen zuerst auf `dev` zu machen**
   - `main` bleibt stabil und sauber.
   - Experimente und neue Features können in `dev` getestet werden.
   - Bessere Nachvollziehbarkeit der Änderungen.

5. **Befehl, um aktuellen Branch zu sehen**
   - `git branch --show-current`
   - oder `git status` (zeigt Branch oben an).

6. **Befehle für Staging & Commit**
   - Staging: `git add <datei>` oder `git add .`
   - Commit: `git commit -m "Beschreibung"`
