---
Summary:
tags:
---
---
## 1️⃣ Verschieben oder Übertragen von Dateien zwischen Branches in **Azure DevOps** (bzw. mit Git generell)

---
Typischer Workflow, den du direkt **lokal** mit Git-Befehlen durchführen solltest. Azure DevOps selbst bietet im Web-UI keinen direkten Button „Datei von Branch X zu Branch Y verschieben“, sondern du arbeitest wie gewohnt mit lokalen Git-Befehlen und pusht dann ins Remote-Repo.

Hier die **Schritte**, um Dateien von deinem Branch `master` (oder `mine`) nach `main` zu übertragen:

### 1. Stelle sicher, dass beide Branches aktuell sind

`git fetch`
### 2. Wechsle zum **Ziel**-Branch (z.B. `main`):

`git checkout main 
`git pull`
### 3. Hole die gewünschten Dateien aus dem **Quell-Branch** (z.B. `master`):

Du kannst **einzelne Dateien** aus einem anderen Branch mit folgendem Befehl übernehmen:

`git checkout master -- pfad/zur/deiner/datei.txt`

Du kannst so auch **ganze Ordner** übernehmen:

`git checkout master -- pfad/zum/ordner/`

_Hinweis:_ Das überschreibt die Datei im aktuellen Branch mit der Version aus `master`.

### 4. Die Datei(en) sind nun in deinem Arbeitsverzeichnis. Füge sie zum Commit hinzu:

`git add pfad/zur/deiner/datei.txt 
`git commit -m "Datei aus master übernommen"` 
`git push`

---

### Tipp: Merge, wenn viele Dateien betroffen sind

Wenn du sehr viele Dateien zwischen den Branches abgleichen möchtest, ist oft ein **Merge** sinnvoller:

`git checkout main git merge master git push`

_Achtung_: Dadurch werden **alle** Änderungen von `master` nach `main` übernommen. Bei Konflikten musst du diese auflösen.