---
tags:
  - Obsidian
  - Plugin
---
---

[Database Folder](https://rafaelgb.github.io/obsidian-db-folder/)

# Problem: Kein Zeilenumbruch

## Schritt-für-Schritt-Anleitung: CSS-Workaround für Zeilenumbruch im DB Folder Plugin

https://www.perplexity.ai/search/ich-benutze-in-obsidian-das-db-lEpB9vKIRi6DY0S7Np6Apw#1

## 1. CSS-Snippet-Datei erstellen

- **Vault-Ordner öffnen**: Navigiere in Obsidian zu `Einstellungen → Erscheinungsbild → CSS-Snippets` und klicke auf das Ordnersymbol (🔗 [3](https://help.obsidian.md/snippets)[4](https://www.reddit.com/r/ObsidianMD/comments/vfucwb/how_do_you_create_a_css_file_and_have_it_go_to/?tl=de)). **Ordner öffnet sich im Explorer.**
- **Neue CSS-Datei anlegen**: Erstelle im `snippets`-Ordner eine Datei namens `db-folder-wrap.css` (Rechtsklick → Neue Datei).
    
## 2. CSS-Code einfügen

Öffne die Datei mit einem Texteditor und füge diesen Code ein:

```css
`.database-plugin__table {   table-layout: fixed;  width: 100%; } .database-plugin__text-nowrap {   white-space: normal !important;  word-break: break-word !important; }`
```

_Hinweis:_ `!important` überschreibt die Standardstyles des Plugins ([1](https://www.reddit.com/r/ObsidianMD/comments/ut6a55/line_breaks/?tl=de)[3](https://help.obsidian.md/snippets)).

## 3. Snippet aktivieren

1. Gehe zurück zu Obsidian
    
2. Aktiviere das Snippet unter `Einstellungen → Erscheinungsbild → CSS-Snippets`
    
3. Klicke auf **Snippets neu laden** (![[lucide-refresh-cw.svg#icon]])
    
4. Aktiviere den Schalter neben `db-folder-wrap.css`
    

## 4. Ergebnis prüfen

- Öffne deine DB Folder-Tabelle
    
- Langer Text sollte nun automatisch umbrechen
    
- Spaltenbreite passt sich automatisch an ([7](https://github.com/RafaelGB/obsidian-db-folder)[8](https://rafaelgb.github.io/obsidian-db-folder/))
    

**Troubleshooting:**

- Bei Mac: Versteckte Ordner mit `Cmd + Shift + .` anzeigen ([4](https://www.reddit.com/r/ObsidianMD/comments/vfucwb/how_do_you_create_a_css_file_and_have_it_go_to/?tl=de))
    
- Funktioniert nicht? Prüfe Doppelpunkt/Semikolon im CSS-Code
    
- Theme-Konflikte: Teste mit Standardtheme (z.B. „Ursprünglich“)
    

Der Workaround bleibt auch nach Plugin-Updates aktiv. Für zukünftige Updates des DB Folder Plugins empfiehlt sich ein gelegentlicher Check, ob der offizielle Zeilenumbruch funktioniert.