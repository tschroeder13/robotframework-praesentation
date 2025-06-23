# Robot Framework Präsentation mit Marp

Dies ist eine codebasierte Präsentation über das [Robot Framework](https://robotframework.org), erstellt mit [Marp](https://marp.app).  
Die Präsentation wird automatisch als HTML-Version generiert und über GitHub Pages veröffentlicht.

## 🔧 Setup & lokale Vorschau

1. Node.js installieren
2. Marp CLI global installieren:

```bash
npm install -g @marp-team/marp-cli
```
3. Präsentation umwandeln:

```bash
marp slides/robotframework.md --html -o dist/index.html
```
4. Lokale Vorschau:

```bash
marp -s slides/
```

## 🚀 Automatischer Build mit GitHub Actions
Bei jedem Push in den main-Branch wird die Präsentation automatisch gebaut und über GitHub Pages bereitgestellt.

## 🌐 Live-Demo
➡ Hier klicken für die Präsentation