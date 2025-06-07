---
tags:
  - GitHub
  - Skills
  - Softwareentwicklung
  - Anleitung
  - Methode
  - Git
  - Agenten
Summary: Anleitung zur lokalen Git-Repository-Erstellung und Veröffentlichung auf GitHub.
---
---
## 🧰 Voraussetzungen

- **GitHub-Konto**: Stelle sicher, dass du ein Konto auf [github.com](https://github.com) hast.
- **Git installiert**: Überprüfe mit `git --version`, ob Git auf deinem System installiert ist.
- **Projektordner**: Du hast bereits einen Projektordner, z. B. `mein-projekt/`, mit der gewünschten Struktur erstellt.

---

## 📝 Schritt-für-Schritt-Anleitung

### 1. 📁 Lokales Git-Repository initialisieren

Öffne dein Terminal und navigiere in deinen Projektordner:

bash

```
cd /pfad/zu/deinem/mein-projekt
git init
```

EXKURS: Mögliche Probleme bei Zeilenumbrüche, daher empfiehlt sich dieser Zwischenschritt um Linux-kompatible Umbrüche für die Arbeit mit WSL zu konfigurieren [[Git Konfiguration Zeilenumbrüche (CRLF, LF)]]

---

### 2. 📄 `.gitignore` erstellen

Erstelle eine `.gitignore`-Datei, um Dateien und Ordner vom Tracking auszuschließen:

bash

```
echo ".venv/" >> .gitignore 
echo "__pycache__/" >> .gitignore 
echo ".env" >> .gitignore
```

### 3. 📤 Dateien zum Commit hinzufügen

bash

```
git add . 
git commit -m "Initialer Commit"
```


### 4. 🌐 Neues Repository auf GitHub erstellen

1. Melde dich bei [GitHub](https://github.com) an.
2. Klicke oben rechts auf das **Plus-Symbol (+)** und wähle **"New repository"**.
3. Gib einen **Repository-Namen** ein, z. B. `mein-projekt`.
4. Optional: Füge eine Beschreibung hinzu.
5. Wähle die Sichtbarkeit: **Public** oder **Private**.
6. ==**Wichtig**: **Deaktiviere** die Optionen für README, `.gitignore` und Lizenz, da du diese bereits lokal hast.== Sonst gibt es fiese Konflikte
7. Klicke auf **"Create repository"**.
    

### 5. 🔗 Lokales Repository mit GitHub verbinden

GitHub zeigt dir nach der Erstellung des Repositories die Befehle an. Führe diese im Terminal in VS Code aus:

bash
```
git remote add origin https://github.com/pssah4/REPOSITORY-NAME.git 
```
```
git branch -M main 
```
```
git push -u origin main
```

Ersetze `dein-benutzername` mit deinem GitHub-Benutzernamen (hier: pssah4, oder unter Code-Button im Repo den Link abrufen)

---

## ✅ Ergebnis

Dein Projekt ist nun auf GitHub verfügbar unter:

arduino

`https://github.com/dein-benutzername/mein-projekt`

Du kannst es mit anderen teilen oder weiterentwickeln.

---

## 📘 Weiterführende Ressourcen

- [GitHub Docs: Neues Repository erstellen](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)
- [GitHub Docs: Projekt auf GitHub hochladen](https://docs.github.com/en/get-started/start-your-journey/uploading-a-project-to-github)