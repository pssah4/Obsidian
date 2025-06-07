---
Summary: Schrittweise Einrichtung einer Python-Dev-Umgebung mit venv in VS Code.
tags:
  - Python
  - VSCode
  - Entwicklungsumgebung
  - VirtualEnvironment
  - Docker
  - Projektstruktur
  - Scripting
  - Automatisierung
  - Softwareentwicklung
  - Git
  - Projektsetup
---
---
# Automatisiertes Setup für eine Python-Entwicklungsumgebung mit venv und src-Struktur

---
## 1.1 Setup-Skript **mit Git-Initialisierung:** create_project.sh`

Dieses Skript richtet eine neue Python-Projektstruktur **inklusive Git-Initialisierung** ein.
```bash
#!/bin/bash

# Projektname als Argument
PROJECT_NAME=$1

if [ -z "$PROJECT_NAME" ]; then
  echo "❌ Bitte gib einen Projektnamen an: ./create_project.sh mein-projekt"
  exit 1
fi

# Projektstruktur anlegen
mkdir -p "$PROJECT_NAME/src/tools"
cd "$PROJECT_NAME" || exit 1

# Virtuelle Umgebung einrichten
python3 -m venv .venv

# Grunddateien
touch requirements.txt .env README.md

# .gitignore
cat <<EOF > .gitignore
.venv/
__pycache__/
.env
EOF

# .gitattributes
cat <<EOF > .gitattributes
* text=auto eol=lf
EOF

# .editorconfig
cat <<EOF > .editorconfig
root = true

[*]
charset = utf-8
end_of_line = lf
insert_final_newline = true
trim_trailing_whitespace = true
indent_style = space
indent_size = 4
EOF

# main.py
cat <<EOF > src/main.py
from tools.greet import greet

def main():
    print(greet("Sebastian"))

if __name__ == "__main__":
    main()
EOF

# greet.py
cat <<EOF > src/tools/greet.py
def greet(name):
    return f"Hallo, {name}!"
EOF

# Git initialisieren + Commit
git init
git add .
git commit -m "🧱 Initialer Projektstart mit venv, Struktur, Git, Zeilenenden"

# Erfolgsmeldung
echo ""
echo "✅ Projekt '$PROJECT_NAME' wurde vollständig eingerichtet!"
echo "📂 Struktur:"
echo "   $PROJECT_NAME/"
echo "     ├── .venv/ (virtuelle Umgebung)"
echo "     ├── .gitignore, .editorconfig, .gitattributes"
echo "     ├── README.md, .env, requirements.txt"
echo "     └── src/ (Python-Code)"
echo ""
echo "👉 Starte jetzt mit:"
echo "   cd $PROJECT_NAME"
echo "   source .venv/bin/activate"
echo "   python src/main.py"

```
---
## 1.2 Setup-Skript **ohne Git-Initialisierung:** create_project_no_git.sh`

Dieses Skript erstellt **die identische Projektstruktur**, **ohne** ein neues Git-Repository zu initialisieren oder Dateien zu committen. Ideal, wenn das Projekt schon in einem Git-Repo liegt oder Git explizit nicht verwendet werden soll.
```bash
#!/bin/bash

# Projektname als Argument
PROJECT_NAME=$1

if [ -z "$PROJECT_NAME" ]; then
  echo "❌ Bitte gib einen Projektnamen an: ./create_project_no_git.sh mein-projekt"
  exit 1
fi

# Projektstruktur anlegen
mkdir -p "$PROJECT_NAME/src/tools"
cd "$PROJECT_NAME" || exit 1

# Virtuelle Umgebung einrichten
python3 -m venv .venv

# Grunddateien
touch requirements.txt .env README.md

# .gitignore
cat <<EOF > .gitignore
.venv/
__pycache__/
.env
EOF

# .gitattributes
cat <<EOF > .gitattributes
* text=auto eol=lf
EOF

# .editorconfig
cat <<EOF > .editorconfig
root = true

[*]
charset = utf-8
end_of_line = lf
insert_final_newline = true
trim_trailing_whitespace = true
indent_style = space
indent_size = 4
EOF

# main.py
cat <<EOF > src/main.py
from tools.greet import greet

def main():
    print(greet("Sebastian"))

if __name__ == "__main__":
    main()
EOF

# greet.py
cat <<EOF > src/tools/greet.py
def greet(name):
    return f"Hallo, {name}!"
EOF

# Erfolgsmeldung
echo ""
echo "✅ Projekt '$PROJECT_NAME' wurde vollständig eingerichtet (ohne git init)!"
echo "📂 Struktur:"
echo "   $PROJECT_NAME/"
echo "     ├── .venv/ (virtuelle Umgebung)"
echo "     ├── .gitignore, .editorconfig, .gitattributes"
echo "     ├── README.md, .env, requirements.txt"
echo "     └── src/ (Python-Code)"
echo ""
echo "👉 Starte jetzt mit:"
echo "   cd $PROJECT_NAME"
echo "   source .venv/bin/activate"
echo "   python src/main.py"
```

---
## 2. **Verwendung beider Skripte**

**Wähle das passende Skript aus und führe es aus**: Wie man das Git Repo in Azure DevOps mit VS Code in der WSL verbindest: siehe [[VS Code & Azure DevOps Repo via SSH (WSL & Symlink)]]

```bash
chmod +x create_project.sh           # oder create_project_no_git.sh
./create_project.sh mein-projekt     # oder ./create_project_no_git.sh mein-projekt
cd mein-projekt
source .venv/bin/activate
python src/main.py
```
---
## 3. Erläuterung der erzeugten Projektstruktur und Dateien

Nach Ausführung eines der Skripte findest du diese Struktur:
```bash 
mein-projekt/
├── .venv/                # Virtuelle Python-Umgebung (nur für dieses Projekt)
├── src/                  # Dein Projektcode
│   ├── main.py           # Einstiegspunkt des Projekts
│   └── tools/
│       └── greet.py      # Beispiel-Modul
├── requirements.txt      # Liste der Python-Abhängigkeiten
├── .env                  # Secrets und API-Keys (niemals in Git einchecken!)
├── .gitignore            # Git: ignoriert z. B. .venv, __pycache__, .env
├── .gitattributes        # Git: Konfiguration für Zeilenenden etc.
├── .editorconfig         # Editor: Vereinheitlicht Formatierung
└── README.md             # Projektbeschreibung

```
#### **Erläuterungen zu den wichtigsten Elementen**

- **`.venv/`**  
	Isolierte Python-Umgebung. Hier liegen Interpreter, Pip und installierte Pakete.  
	→ **Soll nie in Git eingecheckt werden** (siehe `.gitignore`), da venv sehr groß sein kann, abhängig vom Betriebssystem ist und nur eine Laufzeitumgebung darstellt.

- **`src/`**  
    Hier gehört ausschließlich dein Projektcode hin.
      - **`main.py`**: Einstiegspunkt (Startdatei) deines Programms
      - **`tools/`**: Beispiel für eigene Module, z.B. für Utility-Funktionen
 
- **`requirements.txt`**
	Enthält alle Paket-Abhängigkeiten und wird von allen im Projekt gebraucht, z.B.:
	```nginx
	gradio 
	pandas 
	requests
	```
   **Installation aller Pakete:**
```bash
  pip install -r requirements.txt
```
- **`.env`**  
    Für Passwörter, API-Schlüssel usw.  
    → **Nie committen!** (steht in `.gitignore`)

- **`.gitignore`**  
    Listet alles auf, was Git ignorieren soll (z. B. `.venv/`, `__pycache__/`, `.env`).

- **`.gitattributes`**  
    Stellt einheitliche Zeilenenden und Datei-Attribute für Git sicher.

- **`.editorconfig`**  
    Erzwingt eine einheitliche Editor-Formatierung im Team (z. B. Tabs vs. Spaces).

- **`README.md`**  
    Projektbeschreibung, Hinweise, Installationsanleitung, Beispiele usw.


---
## 4. Warum diese Struktur? (Best Practice & Vorteile)

- **Isolierte Umgebung:** Verhindert Konflikte durch Abhängigkeiten anderer Projekte.

- **Saubere Trennung:** Code liegt **immer** in `src/`, Umgebungsdaten und Metadaten bleiben außen vor.
   
- **Klares Git-Handling:** `.venv` und sensible Daten wie `.env` landen nie im Repository.
   
- **Schneller Einstieg:** Sofort nutzbare Struktur, keine manuellen Schritte nötig.
   
- **Teamfähigkeit & Erweiterbarkeit:** Einheitliche Formatierung und klar getrennte Zuständigkeiten (Code, Doku, Meta).

---
## 5. Häufige Workflows & Tipps

- **Projekt initialisieren:**  
    Skript ausführen, wie oben beschrieben.
   
- **Pakete installieren:**  
    ‼️In aktivierter venv:
        ```bash
    	pip install <paketname>
    	pip freeze > requirements.txt   # um requirements.txt zu aktualisieren
    ```
- **Projektbeschreibung pflegen:**  
Immer relevante Hinweise, Installation und Usage in `README.md` dokumentieren.

> [!warning] Achtung
> **Nie .env und .venv in Git pushen!**  Das schützt sensible Daten und sorgt für reproduzierbare Setups.


---

## 6. Erweiterungen

Du kannst die Skripte anpassen, z. B.:

- Zusätzliche Ordner wie `tests/` anlegen
- Vorlagen für weitere Module oder Notebooks erzeugen
- Einen Standard-Dockerfile hinzufügen (außerhalb von `src/`)
- Spezielle Python-Versionen im Skript abfragen

---

**Fazit:**  
Mit diesen Skripten und der sauberen Struktur bist du sofort arbeitsfähig, schaffst einheitliche Standards und vermeidest typische Stolperfallen beim Projektstart – egal ob mit oder ohne Git-Initialisierung.












































# **Startpunkt: Wie denkt ein Entwickler bei einem neuen Projekt?**

1. Ich brauche eine isolierte Umgebung → `venv`
2. Ich muss Pakete sauber verwalten → `requirements.txt`
3. Ich will meine API-Keys/Secrets nicht im Code speichern → `.env`
4. Ich will den Code strukturieren und wiederverwenden → `src/`
5. Ich brauche Git für Versionierung → `.git`, `.gitignore`
6. Ich will eine zentrale Startdatei → `main.py` 
7. Ich brauche eine Projektbeschreibung → `README.md`

## **Schritt-für-Schritt Aufbau in VS Code mit WSL**

Template in VS Code: "C:\Code\Setup_template"

### **1. Projektordner erstellen**

bash (Terminal)

`cd ~` 
``mkdir mein-projekt`
`cd mein-projekt`

### **2. Virtuelle Umgebung einrichten**

bash (Terminal)

`python3 -m venv .venv 
`source .venv/bin/activate`

> 💡 Du erkennst die Aktivierung an: `(.venv)` im Terminal
> 
> ![[Pasted image 20250508075113.png]]

![[Pasted image 20250508075231.png]]

#### **.venv/**

Der **virtuelle Projekt-Python** – völlig losgelöst von deinem System-Python.  
Wird mit `python -m venv .venv` erzeugt.

####  **bin/**

**Wichtigster Ordner**: Hier liegen die ausführbaren Dateien der Umgebung:

| Datei                             | Zweck                                                            |
| --------------------------------- | ---------------------------------------------------------------- |
| `activate`                        | Aktiviert die Umgebung in Bash/Zsh (`source .venv/bin/activate`) |
| `activate.csh/fish/ps1`           | Aktivierung für andere Shells (z. B. PowerShell)                 |
| `python`, `python3`, `python3.12` | **Der eigene Python-Interpreter** dieser Umgebung                |
| `pip`, `pip3`, `pip3.12`          | Die eigene Paketverwaltung – unabhängig vom System-Python        |

💡 **Du rufst ab sofort genau diesen `python` und `pip` auf**, wenn die venv aktiviert ist.

#### **include/**

Technisch wichtig, aber für dich meistens egal. Enthält Header-Dateien für C-Extension-Module (z. B. wenn du Python mit nativen Bibliotheken wie NumPy kompilierst).

#### **lib/python3.12/site-packages/

**Hier landen alle installierten Python-Pakete**, wenn du `pip install ...` machst.  
Dein ganz persönliches **Werkzeuglager**.

Beispiel:

bash
`pip install gradio → landet hier drin`

#### **lib64/...

Nur symbolische Links auf `lib/` – technisch wichtig, aber für dich irrelevant.  
Nur da, weil manche Linux-Setups `lib64` brauchen (64bit-Umgebungen).

### **pyvenv.cfg

Konfigurationsdatei für die `venv`.  
Sie enthält Infos wie:

ini

`home = /usr/bin 
`include-system-site-packages = false 
`version = 3.12.2`

Du brauchst sie nie direkt anzufassen.

### **Wichtig für dich als Entwickler**

| Brauchst du jemals ...       | Antwort | Warum?                                |
| ---------------------------- | ------- | ------------------------------------- |
| `bin/activate`               | ✅ Ja    | Aktiviert deine venv                  |
| `python`/`pip` in `bin/`     | ✅ Ja    | Nur über diese installierst du Pakete |
| `site-packages/` öffnen      | ❌ Nein  | Wird von Python verwaltet             |
| `lib/`, `include/` editieren | ❌ Nein  | Niemals notwendig                     |
| `pyvenv.cfg` anpassen        | ❌ Nein  | Nur lesen, nicht ändern               |

---

## **Zusammenfassung**

| Ordner/Datei            | Zweck für dich als Entwickler                   |
| ----------------------- | ----------------------------------------------- |
| `bin/activate`          | venv aktivieren (Bash)                          |
| `bin/python`, `bin/pip` | Dein privater Python & Pip                      |
| `lib/.../site-packages` | Wo deine Pakete landen                          |
| `.venv/`                | Deine abgeschottete, wiederverwendbare Umgebung |

## **Empfehlung für dich als Entwickler:

### Lege deinen Code in den Ordner `src/`**

> Das ist **Best Practice** in der Python-Entwicklung.

#### Beispielstruktur

`mein-projekt/ 
│ 
├── .venv/                     # Virtuelle Umgebung 
├── src/                         # → Hier kommt dein echter Code rein 
│   ├── main.py             # Einstiegspunkt 
│   ├── tools/                # eigene Module 
│   └── agents/             # z. B. Agent-Logik 
├── requirements.txt    # Abhängigkeiten 
├── .env                        # Secrets/API-Keys 
├── .gitignore               # Git-Konfiguration 
└── README.md           # Projektbeschreibung`

---
### Warum `src/`?

| Vorteil                           | Warum es sich lohnt                                           |
| --------------------------------- | ------------------------------------------------------------- |
| Verhindert versehentliche Importe | `import x` funktioniert **nur, wenn du es explizit willst**   |
| Testbar & paketierbar             | Tests, Setup und Deploys sind einfacher                       |
| Klar getrennt: Code vs Meta       | `.env`, `README.md`, `.venv/` nicht vermischt mit deinem Code |
| ✨ Industriestandard               | In Open-Source- und Profiprojekten üblich                     |

### Was kommt also **nicht** in `src/`?

| Datei                         | Bleibt **außerhalb** von `src/` |
| ----------------------------- | ------------------------------- |
| `.env`                        | Nur Konfiguration, kein Code    |
| `.gitignore`                  | Meta-Dateien                    |
| `.venv/`                      | Umgebung                        |
| `README.md`                   | Projekt-Dokumentation           |
| `Dockerfile`, `.dockerignore` | Infrastruktur                   |

---

## Tipp: Wenn du später ein Paket bauen willst …

Dann wird aus `src/` z. B.:

`src/ 
└── meinprojekt/     
	├── __init__.py     
	├── core.py     
	└── tools.py`

Und du kannst sagen:

python

`from meinprojekt.tools import ...`

---
## **Die `venv` ist deine **Laufzeitumgebung**

...nicht dein Code. Sie enthält:

- Python selbst (`python`, `pip`)
- alle installierten Pakete (`site-packages`)
- Shell-Startskripte (`activate`)    
- sonst nichts
☝️ **Nein – dein Code in `src/` liegt **nicht** in der `venv/` – und das ist auch genau richtig so!**

### Dein Code liegt im **Projektordner – z. B. `src/`**

Dort entwickelst du, dort versionierst du mit Git – und das bleibt **vollkommen unabhängig** von der Umgebung, in der er läuft.

---

### Wie funktioniert es dann?

Wenn du in aktivierter venv z. B. Folgendes tust:

bash

`(.venv) python src/main.py`

...dann passiert Folgendes:

1. Der **Python-Interpreter aus `.venv/bin/python`** wird gestartet
2. Er führt **deine Datei `src/main.py` aus**
3. Wenn dein Code auf Pakete zugreift (z. B. `import gradio`),  sucht er diese in der `venv/lib/.../site-packages`
### Beispiel

bash

`mein-projekt/ 
├── .venv/                 ← dein Werkzeugkasten 
├── src/ 
│   └── main.py            ← dein Code 
└── requirements.txt`

In `main.py`:

python

`import gradio print("Hello World!")`

Wenn du `pip install gradio` gemacht hast, ist `gradio` **in `.venv/` installiert** – aber dein **Code bleibt sauber in `src/`**

### Warum ist das gut?

| Vorteil                         | Warum du das willst                  |
| ------------------------------- | ------------------------------------ |
| Klarer Trennung                 | Code ≠ Umgebung                      |
| Kein versehentliches Einchecken | `.venv` kommt nicht in Git           |
| Austauschbar                    | Du kannst `venv` löschen & neu bauen |
| Test- und Produktionsumgebungen | arbeiten mit demselben Code          |
### Entwicklerfaustregel:

> **Code lebt im Projektordner.**
> 
> **Die venv ist nur die Brille, durch die Python diesen Code sieht.**



# **Skript: Projekt mit `src/`-Struktur und `.venv` automatisch erstellen**


## **1. Wo speichere ich `create_project.sh`?**

##### Empfohlen:

In deinem Home-Verzeichnis in WSL (root), z. B.:

bash
`cd ~ 
`touch create_project.sh`

Dann öffnest du es in VS Code oder per Terminal-Editor:

bash
`code create_project.sh

## **2. Inhalt für `create_project.sh` (voll funktionsfähig)**

bash
```
#!/bin/bash

# Projektname als Argument
PROJECT_NAME=$1

if [ -z "$PROJECT_NAME" ]; then
  echo "❌ Bitte gib einen Projektnamen an: ./create_project.sh mein-projekt"
  exit 1
fi

# Projektstruktur anlegen
mkdir -p "$PROJECT_NAME/src/tools"
cd "$PROJECT_NAME" || exit 1

# Virtuelle Umgebung einrichten
python3 -m venv .venv

# Grunddateien
touch requirements.txt .env README.md

# .gitignore
cat <<EOF > .gitignore
.venv/
__pycache__/
.env
EOF

# .gitattributes
cat <<EOF > .gitattributes
* text=auto eol=lf
EOF

# .editorconfig
cat <<EOF > .editorconfig
root = true

[*]
charset = utf-8
end_of_line = lf
insert_final_newline = true
trim_trailing_whitespace = true
indent_style = space
indent_size = 4
EOF

# main.py
cat <<EOF > src/main.py
from tools.greet import greet

def main():
    print(greet("Sebastian"))

if __name__ == "__main__":
    main()
EOF

# greet.py
cat <<EOF > src/tools/greet.py
def greet(name):
    return f"Hallo, {name}!"
EOF

# Git initialisieren + Commit
git init
git add .
git commit -m "🧱 Initialer Projektstart mit venv, Struktur, Git, Zeilenenden"

# Erfolgsmeldung
echo ""
echo "✅ Projekt '$PROJECT_NAME' wurde vollständig eingerichtet!"
echo "📂 Struktur:"
echo "   $PROJECT_NAME/"
echo "     ├── .venv/ (virtuelle Umgebung)"
echo "     ├── .gitignore, .editorconfig, .gitattributes"
echo "     ├── README.md, .env, requirements.txt"
echo "     └── src/ (Python-Code)"
echo ""
echo "👉 Starte jetzt mit:"
echo "   cd $PROJECT_NAME"
echo "   source .venv/bin/activate"
echo "   python src/main.py"
```

## **Ausführen des Projekt-Erstellers `create_project.sh`**

Um ein neues Projekt anzulegen, folgen Sie diesen Schritten:

1. **Ausführbar machen** Zuerst muss das Script ausführbar gemacht werden:

```
chmod +x create_project.sh
```

2. **Projekt erstellen** Führen Sie das Script mit einem Projektnamen aus:

```
./create_project.sh name-projektordner
```
2. **In das Projekt wechseln** Nach erfolgreicher Erstellung folgen Sie den angezeigten Anweisungen:

```
`cd mein-neues-projekt
	`source .venv/bin/activate`
    `python src/main.py`
```

Das Script wird dann:

- Einen neuen Projektordner erstellen
- Eine virtuelle Python-Umgebung einrichten
- Grundlegende Dateien und Struktur anlegen
- Git initialisieren
- Eine Übersicht der erstellten Struktur anzeigen

Sie erhalten eine Bestätigung wie diese:

```
✅ Projekt 'mein-neues-projekt' wurde vollständig eingerichtet!
📂 Struktur:
   mein-neues-projekt/
     ├── .venv/ (virtuelle Umgebung)
     ├── .gitignore, .editorconfig, .gitattributes
     ├── README.md, .env, requirements.txt
     └── src/ (Python-Code)
```

---

# Die Konfiguration mit `requirements.txt`

Bei dieser Datei handelt es sich um eine Konfigurationsdatei. Im Prinzip speicher ich dort Werte und greife dann später auf diese zu. Zum Beispiel bei der Insatllation von Paketen.

Wenn ich folgende `requirements.txt` habe, die Pakete auflistet:
```
markdownify
smolagents==1.9.2
requests
duckduckgo_search
pandas
smolagents[gradio]
huggingface_hub>=0.19.0
```
Dann kann ich diese auslesen und alle auf einmal in meiner venv installieren:

Terminal
`pip install -r requirements.txt`