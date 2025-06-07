---
Summary: Azure DevOps Repo via SSH in WSL und VS Code einrichten
tags:
  - Softwareentwicklung
  - Git
  - DevOps
  - Skill
  - Automatisierung
  - Azure
  - VSCode
  - Workflow
  - ITAdministration
  - Anleitung
---
---

| Voraussetzung                 | Ort              | Schritt                                               |
| ----------------------------- | ---------------- | ----------------------------------------------------- |
| Azure DevOps Repo vorhanden   | **Browser**      | Neues leeres Repo anlegen, **SSH-Clone-URL** kopieren |
| Projektordner lokal vorhanden | **WSL-Terminal** | Projekt bereits in WSL angelegt                       |
| Git in WSL installiert        | **WSL-Terminal** | Prüfen mit: `git --version`                           |
| **SSH-Key für Azure DevOps**  | **WSL-Terminal** | Generieren & in DevOps hinterlegen (siehe unten)      |

---

# Schritt-für-Schritt-Anleitung

---
## 1️⃣ **SSH-Key in WSL erzeugen und in Azure DevOps eintragen**

---
### WSL-Terminal


> [!tip] Copy & Paste Probleme
>Wenn Copy & Paste nicht funktioniert liegt das an sogenannten „geschützten Leerzeichen“ (Unicode U+00A0) statt eines normalen Leerzeichens (U+0020). Das Terminal erkennt dadurch den Befehl nicht. **So behebst du das Problem:** Lösche die Leerzeichen im Terminal und tippe sie neu ein.

Generate a private/public key pair
```
ssh-keygen -t rsa
```
Viewing Your Public Key
To display your public key (which you'll need for Azure DevOps configuration):
```
cat .ssh/id_rsa.pub
```
→ **Public Key in Zwischenablage kopieren**

> [!info] Note
> While the passphrase can be empty, using one is strongly recommended
> The passphrase works with the key file to provide two-factor authentication	Remember: You'll need to enter the passphrase once per sync and twice with every commit

---
### Browser → Azure DevOps Web-UI > User Settings > SSH Public Keys

- Öffne das Repo in Azure DevOPs: https://dev.azure.com/enbw/_usersSettings/keys to add your SSH public key
- Clone > SSH > Manage SSH Keys > New Key
- Key einfügen & speichern

---
### WSL-Terminal: Verbindung testen 

Verify your connection to DevOps with:

```
ssh -T git@ssh.dev.azure.com
```
 Antwort: `remote: Shell access is not supported.` zeigt, dass die Verbindung steht.

---
## 2️⃣ **Projektordner als Git-Repo einrichten und initial pushen**

---
### **Wo sollte der Projektordner liegen?**

**Empfohlene Orte:**

**Innerhalb von WSL/Linux**, z. B. unter deinem Home-Verzeichnis:  

   `~/dev/` oder `~/projects/`

Das sorgt für beste Performance und Kompatibilität (insbesondere mit Git, Python, Docker etc.).

**Struktur-Beispiel:**

`~/dev/azuredevops/` 
`~/dev/azuredevops/<projektname>/`

**Alternative:**  
Wenn du unbedingt Windows-Programme auf die Daten zugreifen lassen willst, kannst du auch einen Symlink zu einem Ordner in `/mnt/c/...` nutzen. Für alle reinen Dev-Workflows bleibst du aber besser in `~/dev/...`. 

**→ Siehe unten, Abschnitt Symlink**

---
### **Wie legst du den Projektordner an?**

#### 1. WSL-Terminal

**Ordnerstruktur erstellen:**
```bash
mkdir -p ~/dev/azuredevops/<projektname> 
cd ~/dev/azuredevops/<projektname>
```
 Das `-p` sorgt dafür, dass alle übergeordneten Ordner automatisch mit angelegt werden.
   
#### 2. VS Code

Öffne den Ordner direkt:
```bash
code .
```
oder im VS Code-Menü: **File → Open Folder...**

#### 3. **Ab hier arbeitest du IMMER im Terminal in diesem Ordner.**

- Hier kannst du jetzt ein neues Git-Repo initialisieren (`git init`), ein Python-Projekt anlegen usw.
- Das ist dein „Projektstamm“ für alles, was du mit Git verwalten möchtest.

---
### WSL-Terminal

#### Ins Projektverzeichnis wechseln:
```bash
cd ~/dev/meinprojekt
```
#### Prüfen, ob schon Git-Repo:
```bash
git status
```
Falls nicht:
```bash
git init
```
#### Git-User konfigurieren:
```bash
git config --global user.email "se.hanke@enbw.com"
git config --global user.name "Sebastian Hanke"
```
#### Creating a Repository Directory

Create a dedicated directory for your git repositories:
```bash
mkdir ~/gitrepos
```
#### Azure DevOps SSH-Remote setzen:  
(Siehe Azure DevOps, "Clone" → "SSH")
```bash
git remote add origin git@ssh.dev.azure.com:v3/ORG/PROJEKT/REPO
```
#### Erste Version committen und pushen:

Es muss eine Datei im Ordner liegen, sonst funktioniert der erste commit nicht, z.B. `README.txt`
```bash
git add .
git commit -m "Initial commit"
git push -u origin main
```
---
## 3️⃣ **Repo von Azure DevOps via SSH clonen**

---

### WSL-Terminal

**In Zielordner wechseln:**
```bash
cd /pfad/wo/du/das/repo/haben/willst # Beispiel: cd ~/dev
```
**Clonen:**
```bash
git clone git@ssh.dev.azure.com:v3/ORG/PROJEKT/REPO 
cd REPO
```
> [!tip] Title
> - Du kannst **git clone** und **git push** in `/mnt/c/...` machen
> - Aber: Performance ist in `/home/username/...` (also rein in Linux-WSL) meist besser (bei größeren Projekten).


---

## 4️⃣ **(Optional) Projekt im Windows-Dateisystem verlinken (Symlink)**

---

Wenn du das Repo für **Windows & Linux gleichzeitig** nutzbar machen willst (z.B. zur Bearbeitung in beiden Welten):

Wenn man einen Symlink setzt, passiert Folgendes:

- **~/Code** erscheint im Linux-Dateisystem (WSL) wie ein normaler Ordner,
- **tatsächlich** sind aber alle Inhalte von **C:\Code** (Windows!) sichtbar,
- **Änderungen, die du in ~/Code machst, werden sofort in C:\Code** im Windows-System sichtbar und umgekehrt!
- **Das ist kein Kopieren oder Synchronisieren!**  Der Symlink ist einfach eine „Abkürzung“. Alles, was du im Symlink-Ordner speicherst, wird **direkt** im Ziel-Ordner gespeichert.
- **Es gibt nur _einen_ physischen Ordner** (z.B. C:\Code). Der WSL-Symlink bietet nur einen alternativen Zugang dazu.
- **Umgekehrt funktioniert das NICHT:**  Ein Symlink in Windows (mit `mklink`) zeigt **nicht** automatisch auf einen WSL-Linux-Ordner (außer mit Tricks).  Aber in WSL kannst du alles, was unter `/mnt/c/...` liegt, immer erreichen.
- Ein **Symlink** in WSL (z. B. `~/Code` → `/mnt/c/Code`) ist einfach nur ein alternativer Zugang. **Du kannst jederzeit zurück in deinen normalen WSL-Projektordner wechseln und dort weiterarbeiten.**
- 
---

#### WSL-Terminal

**Symlink setzen:**

`ln -s /mnt/c/Code ~/Code`

→ Nun zeigt `~/Code` auf `C:\Code` (Windows). 

**In WSL einfach:**

`cd ~/Code`

**Beachte:**

- Performance in `/home/username` (rein WSL) ist besser als `/mnt/c/…`!
- Für Build-heavy oder große Projekte **immer Linux-Teil bevorzugen**.einen Symlink setzt, dann passiert **Folgendes:**

---
## 5️⃣ ‼️**Projekt in VS Code öffnen**

---

### WSL-Terminal

`code .`

oder
#### VS Code

File → Open Folder... → Repo-Ordner auswählen

---

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

