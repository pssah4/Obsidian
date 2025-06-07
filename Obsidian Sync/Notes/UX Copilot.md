---
Nutzung: Test
Kategorie: Designing Agent
Verwendung: Prompt basierter UI-Design-Agent mit Figma Integration
URL: https://uxpilot.ai/
tags:
  - UX
  - UI
  - VibeCoding
  - Prompting
  - AI
  - Tools
  - VibeDesigning
  - Technologie
  - Anleitung
Kosten/Monat: 29,00 $/Monat
Aktives_Abo: Nein
Toolbox: true
---
---
# Vibe Designing mit UX Copilot, Figma und ChatGPT

# Funktion/Zweck des Tools "UX Pilot"

UX Pilot ist ein browserbasiertes AI Tool, mit der Prompt-Basiert UI's erstellt werden können. 
Test des Tools anhan
d der UI für das Project "Mosaic", wo ein Nutzerdurch einem dreistufigen Checkoutprozess für Daten geführt wird. https://uxpilot.ai/

Testprojekt in UX Pilot: https://uxpilot.ai/s/c11f046843b1fd42ba316c9bc0297ffa
Testprojekt in Figma: https://www.figma.com/design/xYeK9jT8lbXOrH2yTC7aAA/Mosaic-Publish-Workflows---Finetuned?node-id=12-237&t=NMmN3yGemm4trxr1-1


---
# **1. Setup Figma**

---
## 1.1 Eigenes privates Projekt in Figma anlegen

- Zum Datei-Browser wechseln:
- Melde dich bei Figma an. Klicke ggf. oben links auf das Figma-Logo, um in den Datei-Browser zu gelangen.

---
## 1.2 Team auswählen (falls vorhanden):

- In der linken Seitenleiste siehst du unter „Teams“ deine Teams. Wähle das Team aus, in dem du das Projekt anlegen möchtest. 
- Workspace EnBW > "+ Team" (privates Team anlegen)

---
## 1.3 Neues Projekt erstellen:

- Klicke im gewählten Team auf „+ Projekt“.
- Gib dem Projekt einen Namen (z.B. „Mein privates UI-Projekt“).
- Klicke auf „Weiter“ oder „Erstellen“.
- Füge keine weiteren Personen hinzu, wenn es privat bleiben soll.

---
## 1.4 Design System klonen, um unabhängig zu arbeiten

---
### 1.4.1 Design System-Datei im Datei-Browser finden

1. EnBW Design System: [UI_UX ENBW - Design System V2.0 – Figma](https://www.figma.com/design/oLhgJFiyCl9XiLum6fnBr5/UI_UX-ENBW---Design-System-V2.0?node-id=904-15289&p=f&t=Tf20WicOSBTwBZDw-0)
2. Datei duplizieren (klonen):
3. Rechtsklick auf die Design System-Datei.
4. Wähle „Duplizieren“ (englisch: „Duplicate“).
5. Wenn du nur Leserechte hast, wird die Kopie automatisch in deinen „Entwürfen“ (Drafts) gespeichert.
6. Die Kopie trägt den Namen [UI_UX ENBW - Design System v2.0 (copy)]()

---
### 1.4.2 Kopie ins eigene Projekt verschieben:

1. Gehe in deine „Entwürfe“ (Drafts).
2. Ziehe die kopierte Datei per Drag & Drop in dein neues privates Projekt im Team oder nutze das Kontextmenü („Verschieben in...“).

---
### 1.4.3 Mit dem geklonten Design System arbeiten:

1. Öffne die kopierte Datei im Projekt.
2. Du kannst jetzt Komponenten, Styles und Assets beliebig nutzen und bearbeiten, ohne das Original zu verändern

---
# **2. UX Pilot Wireframes erstellen** 


> [!info] SEHR WICHTIG
> > Bevor man Komponenten (max. 100) aus dem Design System nach UX Pilot importiert, benötigt man eine Vorstellung vom Design, um die notwendigen Komponenten aussuchen zu können. Ein notwendiger Schritt vor Erstellung der Hifi Designs ist daher die Erstellung von einfachen Wireframes (direkt in UX Pilot, ohne Figma Plugin) und Ausarbeitung des User Flows.

---
## 2.1 Wireframes auf UX Pilot Website erstellen

Auswahl: 
- Wireframes
- Screen Type: Desktop
- Standard Model (May 2025)
- Deep Design: on

Die UX Pilot Website ist für die Erstellung die besser Option, da es mehr Möglichkeiten gibt (z.B. Hinzufügen von Referenzen und Bildern, die nachgebaut werden).

---
## 2.2 Initialer Context Prompt

```
User Flow for publishin Notes in Obsidian Note-taking Tool

Purpose: AI agent-supported 3-step wizzard to guide users in publishing data and ensure data quality, to guide users through publishing data efficiently and ensure data quality, all communicated in German.

UI Components:
- Visual illustration of the user flow, highlighting the current step in the process. 
- Required steps and screens for the workflow: "Daten auswählen", "Qualitätsprüfung", "Daten teilen". 
- AI Assistant that checks issues and makes suggestions to fix them or offers to fix them directly

Style:
- modern, functional, minimalistic, business oriented, structured and user friendly
- Consistent design. The style is reminiscent of modern enterprise or SaaS applications
- Check spacing and size of components and elements for a premium appearance

Interaction design & UX:
- The user is guided through a 3-step wizard
- Helpful assistance functions: AI suggestions with decision options (clearly visible but not intrusive). 
- Place the "Copilot" below the main section
- No Preview section in on the screen
- Quick access (tags, preview, etc.) are grouped sensibly
```

Bei ```Create Flow``` habe die Option ```Auto Flow``` ausgewählt und von den 5 automatisch generierten Screens diese 3 behalten:

```
Erster Schritt des Wizards, in dem Benutzer die zu veröffentlichenden Daten auswählen können.
```

```
Zweiter Schritt des Wizards, der Nutzern hilft, die ausgewählten Daten auf Qualität und Fehler zu überprüfen, unterstützt durch den KI-Assistenten.
```

```
Dritter Schritt des Wizards, in dem Benutzer die geprüften Daten teilen können, mit Unterstützung durch den KI-Assistenten für zusätzliche Optionen und Empfehlungen.
```

---
### Ergebnis:

![[Pasted image 20250527163258.png]]

![[Pasted image 20250527163248.png]]

![[Pasted image 20250527163330.png]]

---
## 2.3 Finetuning der einzelnen Screens

Auswahl von Global Edit oder Section Edit in Menüleiste der Frames:

![[Pasted image 20250527163548.png]]

---
### **Screen 1**

- Text Edits im gesamten Screen: Funktioniert noch nicht gut, nehme ich später in Figma vor.
- Section Edits mit Prompts

```
Prompt:

- Data selection is only for foles, not for folders.
- search is for notes and/or tags
- no dropdown for selelction next to the search box
- remove tags button next to search box
```

```
Prompt:

- Rename Copilot to Mosaic Copilot
- On first screen, copilot checks for:
- if published note contains backlinks that are not published yet (to avoid dead links after publishing)
- files (png, jpg, pdf etc) attached to the note that are not published to avoid dead links after publishing
- all other issues are handled in the next screen (quality check)
- Copilot suggest fix (publish missing files together with note)
```

---
### **Ergebnis Screen 1:**

![[Pasted image 20250527164845.png]]

---
### **Screen 2**

- Text Edits im gesamten Screen: Funktioniert noch nicht gut, nehme ich später in Figma vor.
- Section Edits mit Prompts

```
Prompt:

- Quality check is file by file. If more than on efile is selected to be published, this steps repeads for each file. Show on top, for which file current quality check is done and whci other files are remaining to be checked.

The Copilot checks for the following quality problems:

A. Copliot checks, if the note has added properties to the notes. Properties include:
1. Tags (mandatory):
- tags are used to connect published notes in a knowledge graph. therefore tags need to represent the high level content and context of the note. if tags are missing or tags are too detailed, copilot makes suggestions to change
- users can also add tags manually.
2. Company or Content  publisher related to this notes (optional), e.g. EnBW
3. Department(s) involved or affected by note (optional)

B. Copilot checks writing style of the note. If the structure of the content does not follow a rough and comprehensible structure, the copilot suggests structuring the note without changing the meaning of the content.

In addition, the copilot may suggest missing aspects or facts that could be added to improve understanding, relevance, actuality or completeness.
```

```
Prompt:

Remove "Eigenschaften bearbeiten" Button in the Properties section. Changes are made by clicking on the properties directly.
```

```
Prompt:

Add a section where Copilot checks if 
- a very similar note (same topic) has already been published. If so, show the Note and ask the USe if he wnats to contribute jhis knowledge to the exiszting note instead (avoid duplicates)
- check if notes exist, taht are strongly related because the contain topics referenced to this note. Copilot makes suggestions to add Backlinks in the not to thes related notes. 
```

```
Prompt:

- In "Ähnliche Notiz gefunden" ad a button that allows the user to open the similar note.
- in the Properties section, ad an option to delete existing entries with one click ("x" attached to the property)
- optimize the spacing of the property section, its too dense and not easy to understand th eoptions the user has
- In the Structure & Style and Improvement section, Add abutton where the user can read a draft of the enhanced note.
```

Im Entwurf gibt es noch eine Section "Obsidian Copilot Section", die sich per Prompt nicht entfernen lässt (wiederhole Fehlermeldung). Wird dann später in Figma erledigt, in der Darstellung hie rschon abgeschnitten.

---
### Zwischenergebnis Screen 2:

![[Pasted image 20250527172813.png]]

```
Prompt:

- The properties section Eigenschaften der Notiz" has too much whitespace. find another layout solution. Make sure that its still good to read and easy to understand. Make sure that action-elements can be differentiated from each other.
- Rename "Notiz" to "Note" in th entire Screen
```

```
Prompt:

- Change "Unternehmen/Publisher" to "Unternehmen (optional)" and format "(optional)" like "(Pflichtfeld)" in the same lighter color.

- Change "Abteilung(en)" to "Abteilung(en) (optional)" and format "(optional)" like "(Pflichtfeld)" in the same lighter color.
```

```
Prompt:

- Change "Notizen" to "Notes" 
- Change "Eigenschaften" to "Properties"
- Optimize the spacing of the Section "Eigenschaften der Note". Create some Space between the existing Tags/content and the improvement suggestions. The current design is too dense.
```

---
### **Ergebnis Screen 2:**

![[Pasted image 20250527181722.png]]

---
### **Screen 3**

- Text Edits im gesamten Screen: Funktioniert noch nicht gut, nehme ich später in Figma vor.
- Section Edits mit Prompts

```
Prompt:

Revise the page.
The page should have the following sections:

#  Display previously checked notes with the option to select them for publication. Behind each note, there should also be a button to view/open the version to be published.

# Select publication location:
- EnBW (public, recommended) -> checkbox
- Dropdown: select another location to choose other repositories for sharing.
Info text below the selection: “Here you can choose who you want to share your notes with. To network EnBW's knowledge, we recommend sharing it with everyone. You can save confidential documents in a protected SharePoint folder and link to it. If your team has its own repository, you can also select it here.”

# Preview of the repositories in which the note will be published (EnBW public and/or one or more Team Repositories), Dropdown "Anderen oder zusätzöochen Ort auswählen"

# Publication conditions
“I hereby confirm that I agree to the following:”
[Checkbox] If “EnBW” is selected, shared notes and files will be accessible to all EnBW employees.
[Checkbox, only displayed if additional or different locations have been selected] If you select other or additional publication locations, shared notes and files will be accessible to everyone who has access to that location.
[Checkbox] By sharing, I agree to the license terms and am aware that other EnBW employees may also edit the file.

Footnote below the checkboxes, separated by a thin line:
“Changes (including deletions) to notes and files are moderated and only accepted and published after the previous contributor has agreed to these changes.”

# Highlighted action box “Ready for publication”
“All quality checks have been successfully completed. Your files are ready for publication.”
Button with icon and text “Publish now” 
```

---
### **Ergebnis Screen 3:**

![[Pasted image 20250527200339.png]]

---
# **3. Design System Komponenten in UX Pilot importieren**

1. Gehe in Figma auf „Plugins“ und starte das Plugin UX Pilot.
2. Figma Designs System (hier: EnBW Bricks) duplizieren und in eigenes Projekt verschieben
3. UX Plot Plugin öffnen
4. Dupliziertes Design System öffnen und "Import comonents" auswählen
5. Wähle im Design System die gewünschten Komponenten (z.B. Buttons, Checkboxen) aus. Einfach mit der Maus markieren, dann Import.
6. Importiere lieber mehrere kleine Gruppen nacheinander, statt alles auf einmal – das sorgt für bessere Performance und Übersichtlichkeit.
7. Lege eine neue Collection an, wenn es keine bestehende gibt

![[Pasted image 20250527115257.png]]

---
## **4. Wireframes in Hifi Design umsetzen**

> [!info] **Wichtig**
> Verwende in UX Pilot (Browser) die selbe Datei/Ansicht, in der sich auch die Wireframes befinden. Nur so kann man im Context-Prompt direkt darauf refernenzieren.

![[Pasted image 20250527215839.png]]

1. Gehe in dein UX Pilot Dashboard und wähle **„Hifi UI Design“** aus der Liste der verfügbaren Tools aus.
2. Im Dropdown-Menü Unter dem Use Case-Typ wähle anstatt des Standard Models nun **"EnBW Bricks"** aus, also das die 100 Komponenten aus dem Design System, die wir zuvor importiert haben. 
3. **Screen Type**: Desktop
4. Um dein bestehendes Wireframe als Referenz zu nutzen, klicke auf **„Reference“** und wähle dein gespeichertes Wireframe aus. Das erste auswähle ist ok, die anderen werden dann auch grundsätzlich angepasst (spätere Anpassungen aber erforderlich)
5. Nutze folgenden Prompt im **Context**-Fenster:

```
Prompt: 

Implement this wireframe 1:1 for all screens and replace placeholders with components from the EnBW Design System. Copy the layout, spacing, types, colors, and structure exactly.
```

6. Behalte die **Create Flow** Schritte aus den Wireframes bei
7. Klicke auf **„Generate“** und warte, bis UX Pilot das HiFi-Design auf Basis deines Wireframes und Prompts erstellt hat.

---
### **Ergebnis Screen 1**

Perfektes Ergebnis, Wireframe 1:1 mit Design System umgesetzt:

![[Pasted image 20250527220847.png]]

---
### 1. Zwischenergebnis Screen 2

Wireframe wurde nicht korrekt umgesetzt:

![[Pasted image 20250527220943.png]]

Daher nehme ich einen "**Section Edit** mit folgendem Prompt vor und wähle bei den Wireframes Screen 2 als Referenz.

```
Prompt:

Implement the referenced wireframe and picture 1:1 and replace placeholders with components from the EnBW Design System.

Copy the layout, spacing, types, colors, and structure exactly. Use colors to show the status anbd indicate changes (ok, improvements, not ok)

Copy all subsections from the wireframe 1:1 and do not add something or leave anything out:

- Subsection "Ähnliche Note gefunden"
- Subsection "Verwandte Notes gefunden"
- Subsection "Properties der Note"
- Subsection "Struktur und Schreibstil"
- Subsection "Empfohlene Ergänzungen"

```

---
### 2. Zwischenergebnis Screen 2

![[Pasted image 20250527224505.png]]

Die Subsection "Empfohlene Ergänzungen" fehlt immer noch, auch nach Ausprobieren verschiedener Prompzt-Varianten.

Weiterer **Global Edit** mit folgendem Prompt, indem ich den Original-Prompt zur Erstellung der Section im Wireframe verwende: 

```
Prompt:

Keep the design and sections as they are.
Below the section "Struktur & Schreibstil", add a section where the copilot suggest missing aspects or facts that could be added to improve understanding, relevance, actuality or completeness.
```

---
### 3. Zwischenergebnis Screen 2

Wie zuvor: Den Abschnitt "Daten Assistent lösche ich später in Figma"

![[uxpilot-design-1748381544940.png]]

Nochmals Finetuning an Komponenten, die im Wireframe nicht ganz gepasst haben:

```
Prompt:

Add navigation buttons
```

---
### **Ergebnis Screen 3**

![[uxpilot-design-1748383350330.png]]

---
### 1. Zwischenergebnis Screen 3

Wireframe wurde nicht korrekt umgesetzt:

![[uxpilot-design-1748381855120.png]]

Daher nehme ich einen "**Section Edit** mit folgendem Prompt vor und wähle bei den Wireframes Screen 3 als Referenz.

```
Prompt:

Implement the referenced wireframe and picture 1:1 and replace placeholders with components from the EnBW Design System.

Copy the layout, spacing, types, colors, and structure exactly. Use colors to show the status anbd indicate changes (ok, improvements, not ok)

Copy all subsections from the wireframe 1:1 and do not add something or leave anything out:

- Subsection "Notizen für Veröffentlichung auswählen"
- Subsection "Veröffentlicungsort auswählen"
- Subsection "Vorschau Veröffentlichungsorte"
- Subsection "Veröffentlichungsbedingungen"
- Subsection/Call to action "Jetzt Veröffentlichen"

```

---
### 2. Zwischenergebnis Screen 3

Alle Vorgaben aus dem Wireframe sind korrekt umgesetzt.

![[uxpilot-design-1748382201542.png]]

Nochmals Finetuning an Komponenten, die im Wireframe nicht ganz gepasst haben:

```
Prompt:

- Remove the label "Anderen oder weiteren Ort Auswählen" above the dropdown, as the labels is laready insight the dropdown.
- Redisign the final publish section with EnBW Design system components.
```

---
### **Ergebnis Screen 3**

![[uxpilot-design-1748382467770.png]]


---

> [!info] Learning 1: **Direkt mit Hifi Design starten**
> Der Umweg über Wireframes in UX Pilot ist unnötig und erzeugt zusätzlichen Aufwand, wenn man Hifi Designs als Ziel hat. Es entstehen dadurch Kostennachteile und Zeitverlust. Das Finetuning kann auch direkt in Hifi Designs vorgenommen werden. Der Aufwand der Überführung ist größer als die direkte Erstellung. Wireframes also nur um sehr grobe User Flows zu zeigen, keine Designideen.

> [!info] Learning 2: **Details in Figma**
> Die Umsetzung und Änderung von kleinen Details ist mit Prompts teilweise sehr frickelig und umständlich. Daher besser diese Anpassungsbedarfe nach dem Export in Figma umsetzen

---
# 5. Übertrag nach Figma 

Die fertigen Designs können mit installiertem UX Pilot Figa Plugin einfach aus dem Browser nach Figma übertragen werden.

---
## 5.1 In UX Pilot

Einfach Button "Safe for Figma" drücken - fertig.

![[Pasted image 20250528000729.png]]

---
## 5.2 In Figma

1. Neues Design erzeugen
2. UX Pilot Plugin öffnen
3. "Saved" auswählen und Design aus UX Pilot auswählen
4. Es werden alle Figma Screen importiert, nicht nur der gespeicherte. Also alle nicht benötigten Screens löschen.

![[Pasted image 20250528001225.png]]

> [!info]
> Der Import funktioniert, allerdings wird das Layout nicht 1:1 übernommen (Spacing und Sizing passt nicht ganz). Es sind nacharbeiten in Figma erforderlich.


---

# 6. Zwischenfazit Zusammenspiel UX Pilot <> Figma

---
##  6. 1 Vorteile & Einsatzmöglichkeiten

- **Extrem schnelle Prototypenerstellung**: Innerhalb von wenigen Minuten vom Konzept zur klickbaren Demo.
- **AI-Unterstützung**: Sowohl beim Erzeugen von Strukturen als auch bei visuellen Details.
- **Figma-Integration**: Reibungslose Zusammenarbeit mit Design-Tools.
- **Iteratives Design**: Änderungen über Chatfunktion, keine manuelle Anpassung nötig.
- **Code-Grundlage**: Erstes HTML/CSS oder React-Code möglich – nützlich für Entwickler:innen.

---
## 6.2 Bewertung & Grenzen

**Stärken**:
- Spart Zeit bei der Erstellung von Interfaces.
- Kann UX-Frameworks / Design Systems automatisch anwenden.
- Ermöglicht rasches Feedback durch Prototyping.

**Schwächen**:
- Feintuning der generierten Designs hängt von Prompt-Präzision ab.
- Spezifisches Branding oder komplexe Interaktionen müssen oft manuell angepasst werden.
- Exportierter Code ist eher als Ausgangspunkt geeignet, nicht für den direkten Produktionseinsatz.

---
## 6.3 Kosten 

> [!info] **Kosten für das Test-Projekt bis Import nach Figma**
> 
> 945 Token oder 73% des monatlichen Budgets. 73% + 29 USD = USD 21. Hierbei ist jedoch zu beachten, dass sehr viel ausprobiert und getestet wurde. Zeitaufwand (mit Testen, Tutorials lesen/anschauen, Test-Dokumentation erstellen) ca. 8 Stunden.
> 

- Prompts werden in Token bezahlt. Monats- oder Jahresabo möglich.
- Kostenlose Subscription für erstes testen vorhanden, aber zu klein um etwas zu designen.
- Token-Verbrauch pro Prompt zwischen 3-20 Token.
- Pro Subscription: 29 USD/ Monat für 1290 Token, Token können nachgekauft werden.


---

# 7. Finetuning in Figma

---

# 8. User Flow und Click-Prototype in Figma

Als nächstes möchte ich in Figma einen USer Flow basierend auf den erstellten Frames erstellen. Hierzu benötige ich Zugriff auf die Daten, um diese ChatGPT zur Verfügung zu stellen.

---
## 8.1 Persönliches Figma API-Token erstellen

1. Melde dich mit deinem Figma-Account an.
2. Klicke rechts oben auf dein Profilbild → **"Settings"**
3. Scrolle zu **"Personal Access Tokens"**
4. Gib einen Namen ein (z. B. `ChatGPT-Access`) und klicke auf **"Generate token"**. Gewählte EInstellungen: Alles Read only, außer Code Connect (No access)
5. Kopiere den Token (er wird **nur einmal** angezeigt!)

Figma Dokumentation: [REST API - Figma](https://www.figma.com/developers/api#authentication)

---
## 8.2 ## File-ID der Figma-Datei finden

1. Öffne die Figma-Datei im Browser.
2. Die URL sieht so aus:

```
https://www.figma.com/file/abc12345XYZ/My-Design-File
```

3. **`abc12345XYZ`** ist die **File-ID** → diese brauchst du für die API-Anfrage.

---
## 8.3 Mit der API auf die Datei zugreifen

JSON -Inhalt mit einem Python-Skript abrufen. Hierfür erstelle ich zunächst ein Python Projekt in VC Code in WSL, um die Abhängigkeiten und Token sauber wiederverwenden zu können. 

[[Setup Dev Umgebung für Python in VS Code]]

```
import os

from dotenv import load_dotenv
import requests
import json
  
# .env laden
load_dotenv()
  
# Werte holen
FIGMA_TOKEN = os.getenv("FIGMA_TOKEN")
FILE_ID = os.getenv("FILE_ID")
OUTPUT_DATEI = "figma_output.json"
  
url = f"https://api.figma.com/v1/files/{FILE_ID}"
headers = {
    "X-Figma-Token": FIGMA_TOKEN
}
  
response = requests.get(url, headers=headers)

if response.status_code == 200:
    data = response.json()
    with open(OUTPUT_DATEI, "w", encoding="utf-8") as f:
        json.dump(data, f, indent=2, ensure_ascii=False)
    print(f"Datei erfolgreich gespeichert unter: {OUTPUT_DATEI}")
else:
    print("Fehler beim Abrufen der Datei:")
    print(f"Status-Code: {response.status_code}")
    print(response.text)
```

Danach ist die JSON Datei verfügbar. 

---
## 8.4 User Flow und Interaktionsanalyse  

Mit der nun verfügbaren JSON erstelle ich in ChatGPT nun einen User Flow:

ChatGPT, GPT-4.1
```
Prompt + JSON File als Kontext:

# Kontext: Die JSON beinhaltet drei Screens eines Tools, das den User Flows für die Veröffentlichung von Notizen im Notiz-Tool Obsidian steuert. Der Benutzer wird bei der Veröffentlichung von Notes unterstützt und die Datenqualität sicherstellt. 

# Bisherige Arbeistschritte zur Erstellung des Designs: Erstellung (Prompting + Bereitstellung Design System, Finetuning) der 3 Frames in UX Pilot -> Import der Frames nach Figma über UX Pilot Plugin -> Weiteres Finetuning der Frames in Figma -> Export der JSON aus Figma -> Bereitstellung der JSON in diesem Chat zur Analyse. Weitere Screens oder Elemente existieren noch nicht. Das Design System ist vorgegeben und steht sowohl in Figma als auch UX Pilot zur Verfügung. # Analysiere diese JSON. Dieses Design ist die Basis und repräsentiert den Zweck des Tools. Das Design ist noch unvollständig, der User Flow ist noch nicht vollständig in Designs abgebildet. 

# Ziel: Als nächstes sollen der User Flow und alle möglichen Interaktionen basierend auf dem vorleigenden Design vollständig beschrieben werden. Basierend auf diesen Initialen Designs wird ein vollständiger User Flow erzeugt. Dieser User Flow wird dann verwendet, um fehlende Screens zu beschreiben und einen Prompt zu verfassen. Mit diesen Prompts werden in UX Pilot die fehlenden Screens erzeugt und wieder nach Figma exportiert. Ziel ist eine vollständige Figma Datei mit allen möglichen Unser Aktionen und Zuständen, die für die Frontend-Entwicklung verwenden werden kann. #Aufgabe: Erstelle und beschreibe einen Workflow zwischen den Tools UX Pilot und Figma (und bei Bedarf ChatGPT), um das Ziel zu erreichen.  
```

Eregbnis:

| Phase                                  | Haupt-Tool        | Schritte                                                                                                                                                                                                              | Deliverables                                          |                                                                                                                                                                                                                                                                                                                   |
| -------------------------------------- | ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Flow-Mapping**                    | ChatGPT           | * Beschreibe jeden Nutzer­schritt in Klartext (Trigger → Aktion → Reaktion). * Markiere **States** (Leer, Valid, Error, Success…).                                                                                    | · Textuelles Flow-Dokument                            | - Describe each user step (**trigger → action → reaction**) in plain language.<br>- Describe technical tasks for interaction between frontend and backend for each user step<br>- Flag UI **states**: _empty / loading / valid / error / success_.<br>- **Output**: Markdown flow‑spec (one subsection per step). |
| **2. Prompt-Gen für UX Pilot**         | ChatGPT           | * Baue pro Screen einen Prompt: – Kontext (Tool-Zweck + Design-System) – Layout-Wunsch (Header, Sidebar…) – State (z. B. Error-Banner) * Halte die Variablenplatz­halter ein (`{title}`, `{errorMsg}` …).             | · Prompt-Bibliothek (`/prompts/*.md`)                 | **One prompt = one screen/state**.<br>- Prompt blocks: _Context_ → _Layout_ → _State_ → _Component tokens_.<br>- Save to `/prompts/*.md`; use variables (`{title}`, `{errorMsg}` …).                                                                                                                              |
| **3. Screen-Erzeugung**                | UX Pilot          | * Generiere Screens mit den Prompts. * Prüfe sofort, ob Design-Tokens greifen (Farben, Radius). * Exportiere **Frames als Figma-JSON** via Plugin.                                                                    | · UX Pilot-Projekt mit neuen Frames · Export-JSON     | - Run prompts; verify design-system tokens apply.<br>    <br>- Batch‑export frames via plugin ⇒ **Figma JSON v0.x** (stable node IDs).                                                                                                                                                                            |
| **4. Import & Auto-Layout-Refine**     | Figma             | * Import-JSON → neue Page „v0.2 Generated“. * Wandle statische Frames in **Components + Variants** um (z. B. Button: Default / Loading / Disabled). * Aktiviere **Auto-Layout** & **Constraints** für Responsiveness. | · Saubere Figma-Page mit Komponenten                  | - Import on page `Draft v0.x Generated`.<br>    <br>- Convert static frames → **Components & Variants**.<br>    <br>- Add **Auto‑layout** + constraints for responsiveness.                                                                                                                                       |
| **5. Interaktive Prototyp-Verlinkung** | Figma             | * Verbinde Frames zu einem klickbaren Prototyp (Start-Flow → Success). * Hinterlege Hotspots für Keyboard-Shortcuts (Esc, Enter).                                                                                     | · Prototype-Flow „Publish Notes“                      | Nutze **named flows** (Figma → Prototype → Flows) für spätere Analytics.                                                                                                                                                                                                                                          |
| **6. QA & Accessibility**              | ChatGPT + Figma   | * ChatGPT-Check: „Finde fehlende States/Error-Cases“. * In Figma: Kontrast-Plugin & WCAG-Lint durchlaufen lassen.                                                                                                     | · QA-Report · Liste zu ergänzender Screens            | Erstelle je fehlendem State sofort einen neuen Prompt (zurück zu Phase 2).                                                                                                                                                                                                                                        |
| **7. Dev-Handoff**                     | Figma + Storybook | * Nutze **Dev-Mode**: Beschriftete Layer, Property-Names = Code-Tokens (`btn-primary`). * Exportiere **Figma Tokens** JSON für CSS/Design-Token-Pipeline. * Verlinke in Storybook ↔ Figma‐URL pro Component.          | · Final Figma-File v1.0 · Tokens.json · Flow-Spec-PDF | Freeze die File-ID; nur noch per Branch/Version duplicate weiterarbeiten.                                                                                                                                                                                                                                         |

Die folgenden Schritte folgen dem von ChatGPT vorgeschlagenen Workflow. https://chatgpt.com/canvas/shared/6836e013ba38819182d6749c293bbff3

---
### **8.4.1 Flow Mapping — ChatGPT** 

(im selben Chat fortsetzen, damit JSON verfügbar ist, Model: o3)
```
Prompt:

Task: Flow Mapping
- Describe each user step (**trigger → action → reaction**) in plain language.
- Describe technical tasks for interaction between frontend and backend for each user step
- Flag UI **states**: _empty / loading / valid / error / success_.
- **Output**: Markdown flow‑spec (one subsection per step).

The 3 screens and their logical flow order are: Daten auswählen -> Qualitätsprüfung -> Daten teilen
```

#### Flow Mapping Ergebnisse:

---
#### **Screen 1: Daten auswählen**

##### Trigger

- Nutzer öffnet den Publishing‑Dialog (z. B. Klick auf „Note veröffentlichen“).
##### Action(s)

1. **System** ruft alle unveröffentlichten Notizen + Metadaten aus Obsidian ab.
2. **User** filtert / sucht / sortiert die Liste.
3. **User** wählt eine oder mehrere Notizen per Checkbox.
#### Reaction(s)

- **loading**: Spinner & Skeleton‑Rows, bis die Liste vorliegt.
- **empty**: Illustration + CTA „Erstelle erst eine Notiz“.
- **valid**: „Weiter“-Button wird aktiv, Count‑Badge zeigt Auswahl.
- **error**: Banner „Fehler beim Laden der Notizen – Wiederholen?“.
- **success**: Klick auf „Weiter“ → Navigation zu Schritt 2.

##### UI‑States

| State   | Sichtbare Hinweise                      |
| ------- | --------------------------------------- |
| empty   | Zero‑State‑Illustration, sekundärer CTA |
| loading | Spinner in Table + Dimmed UI            |
| valid   | Primary CTA aktiv, Selektion‑Badge      |
| error   | Danger‑Banner + Retry‑Button            |
| success | Route‑Change zu _Qualitätsprüfung_      |

---
#### **Screen 2: Qualitätsprüfung

##### Trigger

- Erfolgreicher Übergang aus „Daten auswählen“.

##### Action(s)

1. **System** analysiert ausgewählte Notizen (Ähnliche Notes, Verwandte Notes, Properties, Struktur & Schreibstil, Empfohlene Ergänzungen).
2. **User** sieht Check‑Liste; kann auf Issues klicken, um Details/Auto‑Fix anzuzeigen.
3. **User** löst alle Blocking‑Issues oder akzeptiert Warnungen/Hinweise.

##### Reaction(s)

- **loading**: Progress‑Bar „Analysiere Notizen …“.
- **error**: Card‑List mit rot markierten Fails; CTA „Fehler anzeigen“.
- **valid**: Alle Checks grün → „Weiter“-Button aktiv.
- **success**: Klick „Weiter“ → Schritt 3.

##### UI‑States

| State   | Sichtbare Hinweise                        |
| ------- | ----------------------------------------- |
| loading | Indeterminate Progress‑Bar + Analyse‑Info |
| error   | Red‑Badge, Issue‑List, Tooltip‑Links      |
| valid   | Green‑Badges, Primary CTA aktiv           |
| success | Route‑Change zu _Daten teilen_            |

> **Keine echte „empty“-Variante**, da immer Checks vorhanden sind – lediglich „alles grün“ ≙ valid.

---

#### **Screen 3: Daten veröffentlichen

##### Trigger

- Qualitätsprüfung ohne Blocking‑Issues abgeschlossen.

##### Action(s)

1. **System** zeigt Zusammenfassung (Anzahl Notizen, Sichtbarkeit, Tags).
2. **User** wählt Ziel‑Repository/Team für Veröffentlichung.
3. User bestätigt Veröffentlichungsbedingungen
4. **User** klickt „Jetzt Veröffentlichen“.

##### Reaction(s)

- **loading**: Spinner im CTA, Status „Veröffentliche …“.
- **error**: Toast „Publishing fehlgeschlagen“, Option „Erneut versuchen“.
- **success**: Confirmation‑Modal mit Copy‑Link‑Button („Note wurde veröffentlicht“).

### UI‑States

| State   | Sichtbare Hinweise                  |
| ------- | ----------------------------------- |
| loading | Spinner + Disabled Inputs           |
| error   | Toast + Danger‑Banner               |
| valid   | CTA aktiv, Publikations‑Preview     |
| success | Success‑Modal, Copy‑Link, Close‑CTA |

---
### Globale States & Edge Cases

- **Session Timeout** → Modal „Bitte neu anmelden“
- **API‑Rate‑Limit** → Retry‑Strategy (Back‑off) + Banner
- **Unsaved Changes** → Warn‑Dialog beim Abbruch

---

### **8.4.2 Prompt Generation (ChatGPT) & Screen Generation (UX Pilot)**

ChatGPT, Modell: o3
```
Prompt:

Neben einem UI Design mit Mock-Content pro Screen habe ich nun das eben erstellte Flow Mapping pro Screen:

#### **Screen 1: Daten auswählen** ##### Trigger - Nutzer öffnet den Publishing‑Dialog (z. B. Klick auf „Note veröffentlichen“). ##### Action(s) 1. **System** ruft alle unveröffentlichten Notizen + Metadaten aus Obsidian ab. 2. **User** filtert / sucht / sortiert die Liste. 3. **User** wählt eine oder mehrere Notizen per Checkbox. #### Reaction(s) - **loading**: Spinner & Skeleton‑Rows, bis die Liste vorliegt. - **empty**: Illustration + CTA „Erstelle erst eine Notiz“. - **valid**: „Weiter“-Button wird aktiv, Count‑Badge zeigt Auswahl. - **error**: Banner „Fehler beim Laden der Notizen – Wiederholen?“. - **success**: Klick auf „Weiter“ → Navigation zu Schritt 2. ##### UI‑States | State | Sichtbare Hinweise | | ------- | --------------------------------------- | | empty | Zero‑State‑Illustration, sekundärer CTA | | loading | Spinner in Table + Dimmed UI | | valid | Primary CTA aktiv, Selektion‑Badge | | error | Danger‑Banner + Retry‑Button | | success | Route‑Change zu _Qualitätsprüfung_ | --- #### **Screen 2: Qualitätsprüfung ##### Trigger - Erfolgreicher Übergang aus „Daten auswählen“. ##### Action(s) 1. **System** analysiert ausgewählte Notizen (Ähnliche Notes, Verwandte Notes, Properties, Struktur & Schreibstil, Empfohlene Ergänzungen). 2. **User** sieht Check‑Liste; kann auf Issues klicken, um Details/Auto‑Fix anzuzeigen. 3. **User** löst alle Blocking‑Issues oder akzeptiert Warnungen/Hinweise. ##### Reaction(s) - **loading**: Progress‑Bar „Analysiere Notizen …“. - **error**: Card‑List mit rot markierten Fails; CTA „Fehler anzeigen“. - **valid**: Alle Checks grün → „Weiter“-Button aktiv. - **success**: Klick „Weiter“ → Schritt 3. ##### UI‑States | State | Sichtbare Hinweise | | ------- | ----------------------------------------- | | loading | Indeterminate Progress‑Bar + Analyse‑Info | | error | Red‑Badge, Issue‑List, Tooltip‑Links | | valid | Green‑Badges, Primary CTA aktiv | | success | Route‑Change zu _Daten teilen_ | > **Keine echte „empty“-Variante**, da immer Checks vorhanden sind – lediglich „alles grün“ ≙ valid. --- #### **Screen 3: Daten veröffentlichen ##### Trigger - Qualitätsprüfung ohne Blocking‑Issues abgeschlossen. ##### Action(s) 1. **System** zeigt Zusammenfassung (Anzahl Notizen, Sichtbarkeit, Tags). 2. **User** wählt Ziel‑Repository/Team für Veröffentlichung. 3. User bestätigt Veröffentlichungsbedingungen 4. **User** klickt „Jetzt Veröffentlichen“. ##### Reaction(s) - **loading**: Spinner im CTA, Status „Veröffentliche …“. - **error**: Toast „Publishing fehlgeschlagen“, Option „Erneut versuchen“. - **success**: Confirmation‑Modal mit Copy‑Link‑Button („Note wurde veröffentlicht“). ### UI‑States | State | Sichtbare Hinweise | | ------- | ----------------------------------- | | loading | Spinner + Disabled Inputs | | error | Toast + Danger‑Banner | | valid | CTA aktiv, Publikations‑Preview | | success | Success‑Modal, Copy‑Link, Close‑CTA | --- ### Globale States & Edge Cases - **Session Timeout** → Modal „Bitte neu anmelden“ - **API‑Rate‑Limit** → Retry‑Strategy (Back‑off) + Banner - **Unsaved Changes** → Warn‑Dialog beim Abbruch

Analysiere die States und zusätzlich benötigten Screens. Erstelle für jeden Screen Prompts, um die States im Flow und zusätzlichen Screens in UX Pilot zu generieren. **One prompt = one screen/state**. - Prompt blocks: _Context_ → _Layout_ → _State_ → _Component tokens_. - Save to `/prompts/*.md`; use variables (`{title}`, `{errorMsg}` …).
```

---

#### **Ergebnis:**

In UX Pilot jeweils "Add Screen" bei vorhandenem Screen, dann Prompt. Import nach Figma und geringes Finetuning (Spacing, Icons, Sizes - geringer Aufwand).


> [!info] Hohe Qualität
> Die Ergebnisse sind beindruckend, es ist so gut wie kein Finetuning in Figma mehr erforderlich. 


---
##### **prompts/01_select-data_empty**

```
### Context

Obsidian »Publish Notes« – **Select Data** (Zero‑State). Der Benutzer hat noch keine unveröffentlichten Notizen.

### Layout

- **Step‑Indicator** {stepIndicator} zeigt _1 / 3_ aktiv.
    
- Header {header} mit Headline `{title}` (Bsp.: _„Welche Notizen möchtest du veröffentlichen?“_).
    
- Zentrierte Illustration {illustrationEmpty} & Copy `{bodyText}`.
    
- Primary CTA {primaryButton} → `{primaryButtonLabel}` (_„Neue Notiz erstellen“_).
    

### State

empty

### Component tokens

{stepIndicator}, {header}, {illustrationEmpty}, {primaryButton}
```

![[Pasted image 20250528162904.png]]


---

##### **prompts/02_select-data_loading

```
Prompt:

### Context

Select Data lädt die Liste unveröffentlichter Notizen.

### Layout

- Header + Step‑Indicator identisch zu Empty.
    
- Table‑Skeleton mit 8 Rows {tableRowSkeleton}.
    
- Zentrierter {spinner}.
    
- Suchfeld {searchField} & Filter {filterDropdown} disabled.
    
- Primary CTA disabled.
    

### State

loading

### Component tokens

{stepIndicator}, {header}, {searchField}, {filterDropdown}, {tableRowSkeleton}, {spinner}, {primaryButtonDisabled}
```

![[Pasted image 20250528155244.png]]

---

##### **prompts/03_select-data_valid

```
Prompt:

### Context

Select Data mit geladener Tabelle & aktiver Auswahl.

### Layout

- Header + Step‑Indicator.
    
- Suchfeld {searchField}, Filter‑Dropdown {filterDropdown}.
    
- Table‑Rows {tableRow}: Checkbox {checkbox}, Note‑Title `{noteTitle}`, Modified‑Date, Tag‑Chips.
    
- Selected‑Zähler {badgeCount} zeigt `{noteCount}`.
    
- Primary CTA {primaryButton} „Weiter“ aktiv.
    

### State

valid

### Component tokens

{stepIndicator}, {header}, {searchField}, {filterDropdown}, {tableRow}, {checkbox}, {badgeCount}, {primaryButton}
```

![[Pasted image 20250528161223.png]]


---

##### **prompts/04_select-data_error

```
Prompt:

### Context

Fehler beim Laden der Notizen.

### Layout

- Header + Step‑Indicator.
    
- Error‑Banner {bannerError} mit `{errorMsg}` (_„Serverfehler – versuche es erneut.“_).
    
- Secondary CTA {secondaryButton} „Wiederholen“.
    
- Leere Tabelle ausgegraut.
    

### State

error

### Component tokens

{bannerError}, {secondaryButton}, {primaryButtonDisabled}, {stepIndicator}, {header}
```

![[Pasted image 20250528162055.png]]
---

##### **prompts/05_quality-check_loading

```
### Context

**Quality Check** startet Analyse der ausgewählten Notizen.

### Layout

- Step‑Indicator zeigt _2 / 3_.
    
- Header {header} „Qualitätsprüfung“.
    
- Indeterminate Progress‑Bar {progressBar}.
    
- Copy `{bodyText}` (_„Analysiere {noteCount} Notizen …“_).
    

### State

loading

### Component tokens

{stepIndicator}, {header}, {progressBar}
```

![[Pasted image 20250528162538.png]]

---

##### **prompts/06_quality-check_error**

```
### Context

Analyse ergibt Blocking‑Issues.

### Layout

- Header + Step‑Indicator.
    
- Issue‑Cards {issueCardError}: Title `{issueTitle}`, Badge „Blocker“.
    
- CTA {secondaryButton} „Fehler anzeigen“.
    
- Primary CTA deaktiviert.
    

### State

error

### Component tokens

{stepIndicator}, {header}, {issueCardError}, {secondaryButton}, {primaryButtonDisabled}
```

![[Pasted image 20250528163047.png]]

---

##### **prompts/07_quality-check_valid

(Manuelle Edits, um States zu konkretisieren)

```
### Context

Alle Qualitätskriterien überprüft.

### Layout

- keep design of original screen, show all sections and contents
- use green badges for categories with no findings {issueCardSuccess}.
	example: Category: Ähnliche Notes gefunden: "Keine ähnlichen Notes gefunden"
	Badge „Geprüft“
	use green frame and light green filling

- use yellow badges for categories with findings {issueCard}.
	example: Category: Verwandte Notes gefunden: display notes {same text and layout}
	Badge „Hinweis“
	use yellow frame and light yellow filling


### State

valid

### Component tokens

{stepIndicator}, {header}, {issueCardSuccess}, {primaryButton}

```

![[Pasted image 20250528171323.png]]

---

##### ##### **prompts/08_publish_loading

```
### Context

Publishing in progress.

### Layout
    
- Header {header} „Veröffentlichungung“.
    
- Indeterminate Progress‑Bar {progressBar}.
    
- Copy `{bodyText}` (_„Veröffentliche {noteCount} Notes …“_).
    

### State

loading

### Component tokens

{stepIndicator}, {header}, {progressBar}
```

![[Pasted image 20250528173507.png]]

---
##### **prompts/09_publish_error

```
### Context

Publishing fehlgeschlagen.

### Layout

- Toast {toastError} mit `{errorMsg}`.

- highlight Note or file that causes error
	Badge "Fehler"
	use red frame and light red filling
    
- Danger‑Banner {bannerError}.
    
- Secondary CTA {secondaryButton} „Erneut versuchen“.

- show "Vorschau der Veröffentlichungsorte"
- Do not show Dropdown selection of Veröffentlichungsorte

- highlight Veröffentlichungsort that causes error
	Badge "Fehler"
	use red frame and light red filling

### State

error

### Component tokens

{toastError}, {bannerError}, {secondaryButton}, {primaryButtonDisabled}
```

![[Pasted image 20250528174655.png]]

---

##### **prompts/10_publish_success-modal

```
### Context

Veröffentlichung abgeschlossen.

### Layout
    
- Header {header} „Veröffentlichungung“.
       
- Copy `{bodyText}` (_„Herzlichen Glückwunsch, {noteCount} Notes wurden veröffentlicht!“_).
    

### State

success

### Component tokens
{icon}
```

![[Pasted image 20250528175530.png]]

---
##### **prompts/11_global_session-timeout

(zurückgestellt)
```
### Context

Globale Session‑Timeout‑Warnung.

### Layout

- Full‑Screen Modal {modalSessionTimeout}.
    
- Headline „Session abgelaufen“, Copy `{bodyText}`.
    
- Primary CTA {primaryButton} „Neu anmelden“.
    

### State

global-modal

### Component tokens

{modalSessionTimeout}, {primaryButton}
```

---

##### **prompts/12_global_api-rate-limit

(zurückgestellt)
```
### Context

API‑Rate‑Limit erreicht.

### Layout

- Sticky Banner {bannerError} Top‑of‑App mit `{errorMsg}` (_„Zu viele Anfragen – erneuter Versuch in {retryTime} Sek.“_).
    

### State

global-banner

### Component tokens

{bannerError}

```
---

##### **prompts/13_global_unsaved-changes

(zurückgestellt)
```
### Context

Warnung bei ungespeicherten Änderungen.

### Layout

- Confirmation‑Modal {modalUnsavedChanges}.
    
- Text `{unsavedChangesMsg}`.
    
- Primary CTA {primaryButton} „Verlassen“, Secondary {secondaryButton} „Abbrechen“.
    

### State

global-modal

### Component tokens

{modalUnsavedChanges}, {primaryButton}, {secondaryButton}
```

---
# 9. Prototype Linking — Figma

---
# 10. Dev Handoff

---