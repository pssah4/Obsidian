---
tags:
  - Software
  - Kollaboration
  - Wissensmanagement
  - Git
  - Obsidian
  - Dokumentation
  - ITAdministration
  - Skill
  - Lösung
Summary: Obsidian Vault mit Git-Repository verbinden und synchronisieren.
Nutzung: ""
---
---


## Voraussetzungen

- **Obsidian** installiert
- **VS Code** installiert (empfohlen für Git-Operationen)
- **Git** auf dem Computer installiert
- Zugang zum gewünschten **Git-Repository** (z. B. Link zu GitHub) 

## Schritt 1: Repository klonen

1. Repo in Git anlegen und Dateien dort speichern, siehe auch [[Projekte auf GitHub veröffentlichen]] und [[VS Code & Azure DevOps Repo via SSH (WSL & Symlink)]]
2. **Repository-Link kopieren**, den Link zum gewünschten Git-Repository (z. B. von GitHub oder GitLab) bereithalten.
3. **Ordner wählen/anlegen**: Einen lokalen Ordner auf deinem Computer auswählen oder neu anlegen, in den das Repository geklont werden soll.
4. Lokalen Ordner auswählen, wo die Dateien lokal für VS Code abgelegt werden
5. **Repository klonen**
	- Entweder direkt auf der GitHub/GitLab-Seite den **"Clone in VS Code"**-Button benutzen  
	    **oder**
	- In **VS Code**:
       - Neues Fenster öffnen (`File > New Window`)
       - Im Menü auf **Source Control** (Git-Symbol) gehen
       - Option **"Clone Repository"** wählen und Repository-Link einfügen
       - Zielordner auswählen

![[Git Repositoty auschecken und in VS Clonen.mp4]]

## Schritt 2: Obsidian Vault einrichten

1. Obsidian öffnen
2. In Obsidian neuen Vault anlegen (aus Ordner öffnen)
3. Den Ordner auswählen, in den das Repository geklont wurde

## Schritt 3: Git Plugin in Obsidian installieren

1. Git-Plugin installieren & enablen
2. Meist reicht die Standardkonfiguration, da das Plugin automatisch den `.git`-Ordner erkennt - Optional weitere Einstellungen anpassen (z. B. Synchronisationsintervalle)
3. Obsidian Git-Plugin erkennt automatisch den verborgenen .git Ordner. Anhand dieses Ordners läuft dann der Sync, alle Informationen sind dort enthalten ("Git-Magie")


![[Git-Repo Ordner in Obsidian öffnen.mp4]]

## Schritt 4: Vault und Branches verwalten

- **Branch wechseln (optional)**
    - Im Git-Plugin (oder direkt in VS Code) kannst du den gewünschten Branch auswählen, z. B. `main` oder `feature/*`
- **Vault verwenden**
       - Du kannst nun wie gewohnt mit Obsidian arbeiten
       - Änderungen werden durch das Git-Plugin verfolgt

