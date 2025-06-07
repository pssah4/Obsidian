---
Summary: Anleitung zur lokalen Git-Repository-Erstellung und Veröffentlichung auf GitHub.
tags:
---
---
## Schritt-für-Schritt: Repo auschecken (= clonen)


### 1️⃣ Clone-URL aus Azure DevOps holen

- Gehe in Azure DevOps → Repos → **Clone** → **HTTPS-URL kopieren** 
	Beispiel: `https://dev.azure.com/dein-org/dein-projekt/_git/dein-repo`

---
### 2️⃣ In WSL / VS Code Terminal in Zielordner wechseln

```bash
cd /pfad/wo/du/das/repo/haben/willst # Beispiel: cd ~/dev
```

**Beispiel für Ordner, der lokal liegt C:\Repos\MeinProjekt** → in WSL:

```bash
cd /mnt/c/Repos/MeinProjekt
```
> [!tip] Title
> - Du kannst **git clone** und **git push** in `/mnt/c/...` machen
> - Aber: Performance ist in `/home/username/...` (also rein in Linux-WSL) meist besser (bei größeren Projekten).


---
### 3️⃣ Repo clonen

```bash
git clone https://dev.azure.com/dein-org/dein-projekt/_git/dein-repo
```
→ Jetzt wird ein **Ordner `dein-repo`** erstellt und alles reingeholt.

---
### 4️⃣ In den geklonten Ordner wechseln

```bash
cd dein-repo
```

---
### 5️⃣‼️ In VS Code öffnen (um in dem Ordner/Repo zu arbeiten)

```bash
code .
```

---
### Ergebnis

- Du hast jetzt das Repo **lokal in WSL**
- Es ist **mit Azure DevOps verknüpft**
- Du kannst nun:

`git pull` → Änderungen holen  
`git push` → eigene Änderungen hochladen  
`git add .` → alle Änderungen zum Commit vormerken  
`git add <Dateiname>` → einzelne Datei zum Commit vormerken  
`git commit -m "Kommentar"` → Commit mit Kommentar erstellen  
`git status` → aktuellen Status anzeigen (was ist geändert?)  
`git log --oneline` → Commit-Historie kompakt anzeigen  
`git clone <Repo-URL>` → Repo aus Azure DevOps lokal auschecken  
`git init` → neues Git-Repo initialisieren  
`git remote add origin <Repo-URL>` → Remote-Repo verknüpfen  
`git checkout <Branchname>` → zu Branch wechseln  
`git checkout -b <neuer-Branchname>` → neuen Branch erstellen und wechseln  
`git branch` → lokale Branches anzeigen  
`git branch -a` → alle Branches anzeigen (lokal + remote)  
`git diff` → Unterschiede seit letztem Commit anzeigen  
`git pull origin <Branchname>` → gezielt von Branch Änderungen holen  
`git push origin <Branchname>` → gezielt auf Branch hochladen

---

## **Empfohlene Struktur für Azure DevOps Repos**

### Variante 1: **Im Linux-Teil von WSL (empfohlen)**

→ z.B.:
```bash 
`~/dev ~/projects ~/git/azure`
```
**Beispiel:**

```bash
`~/dev/azuredevops-repo1 ~/dev/azuredevops-repo2`
```

**Vorteile:**  
✅ Schnell  
✅ Keine Zugriffsprobleme  
✅ Git + VS Code laufen hier nativ unter Linux

---
### **Praxis-Tipp für Azure DevOps + WSL**

#### Lege dir in **`~/dev/azuredevops`** einen Ordner an:

```bash
`mkdir -p ~/dev/azuredevops cd ~/dev/azuredevops git clone https://dev.azure.com/...`
```
→ Dann ist alles **super performant** und läuft 100% sauber in VS Code (mit "Remote WSL" Plugin).

#### Zusatz:

Wenn du magst, kann ich dir noch eine **empfohlene Projektstruktur** für **mehrere Azure DevOps Repos** geben — also z.B.:

```bash
`~/dev/azuredevops/repo1 ~/dev/azuredevops/repo2 ~/dev/github/repoX`
```

→ So bleibt es sauber und du findest alles schnell.  
Willst du das auch noch? 🚀

---
### Variante 2: **Im Windows-Dateisystem (z.B. C:)** → `/mnt/c/...`

```bash
`/mnt/c/Repos/AzureDevOps`
```

**Vorteile:**  
✅ Du kannst die Ordner auch im **normalen Windows Explorer** sehen und verwenden  
✅ Einfachere Backups mit Windows-Tools

**Nachteile:**  
⚠️ Langsamer (Datei-I/O über die /mnt/c Brücke)  
⚠️ Manche Tools (Docker, Buildtools) haben Probleme

---
### Variante 3: **Symlink (Verknüpfung von WSL auf C:)

#### Symlink/Verknüpfung erstellen

```bash
ln -s /mnt/c/Code ~/Code
```
Das ist ein **symbolischer Link** (Symlink), also eine Art "virtueller Ordner" oder **Verknüpfung**.

→ Jetzt zeigt `~/Code` auf `/mnt/c/Code`

#### Was bringt das?

Du kannst jetzt in deiner **Linux-Welt (WSL)** arbeiten:

```bash
cd ~/Code
```
→ und landest automatisch in:

```bash
/mnt/c/Code
```

Vorteil:  
✅ Kürzerer Pfad  
✅ Bequemer Zugriff in WSL-Terminal und VS Code  
✅ Gleicher Inhalt → Windows und Linux sehen die gleichen Dateien


### **Schritt für Schritt erklärt** (mit Tipp kombiniert)

#### 🥇 A. Variante 1: **Volle Linux-Performance (empfohlen)**

→ Erstelle **echte Linux-Ordner**, keine Symlinks!
```bash
mkdir -p ~/dev/azuredevops cd ~/dev/azuredevops git clone https://dev.azure.com/...
```
→ Vorteil: super schnell, keine Probleme beim Bauen von Projekten.


#### 🥈 B. Variante 2: **Symlink auf Windows-Ordner (was dein Kollege gemacht hat)**

Wenn du **zwingend** die Projekte **in C:\Code** haben willst:
cd 
```bash
ln -s /mnt/c/Code ~/Code
```
→ Danach kannst du so arbeiten:

```bash
cd ~/Code git pull git push
```

→ Vorteil: Windows und Linux greifen auf den gleichen C:\ Ordner zu.  
→ Nachteil: etwas langsamer, bei komplexen Projekten evtl. Probleme.

---
## Zusammenfassung

| Ziel                                                 | Empfehlung                   |
| ---------------------------------------------------- | ---------------------------- |
| **Entwickeln mit Git, Node, Python, Docker, Builds** | **~/dev** (WSL Linux-Teil)   |
| **Repo nur zum Ansehen / kleine Änderungen**         | `/mnt/c/Repos/...` geht auch |
