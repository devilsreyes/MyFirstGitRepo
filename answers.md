# Antworten zu den Kontrollfragen

### 1. Unterschied zwischen Working Directory, Staging Area und Repository
- **Working Directory:** Dein normaler Arbeitsordner, in dem du Dateien bearbeitest
- **Staging Area: ** Die Zwischenstation (`git add`), um Änderungen für den nächsten Commit vorzumerken
- **Repository: ** Die Git-Datenbank (`.git`), in der alle Commits dauerhaft gespeichert sind

### 2. Woran erkennst du, ob ein Merge Fast-Forward war?
- Im Terminal steht ausdrücklich das Wort **`Fast-forward`**
- Es wird **kein neuer Merge-Commit** erstellt; der Branch-Zeiger rückt einfach weiter

### 3. Warum kann `git merge --ff-only` fehlschlagen?
- Wenn der Ziel-Branch (`main`) in der Zwischenzeit **neue Commits** erhalten hat
- In diesem Fall hat sich die Historie gespalten (divergiert)

### 4. Was ist der Vorteil, Änderungen zuerst auf einem Branch wie `dev` zu machen?
- Der Hauptbranch (`main`) bleibt dauerhaft stabil und funktionsfähig
- Fehler oder unfertige Features stören die Hauptversion nicht

### 5. Mit welchem Befehl siehst du den aktuellen Branch?
- **`git branch`** (der aktive Branch ist mit einem Stern `*` markiert) oder **`git status`**.

### 6. Mit welchen Befehlen machst du Änderungen sichtbar und dauerhaft?
- **Sichtbar / Vormerken (Staging): ** `git add <dateiname>`
- **Dauerhaft speichern (Commit): ** `git commit -m "deine nachricht"`
