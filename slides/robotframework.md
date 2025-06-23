---
marp: true
theme: rose-pine-moon
paginate: true
headingDivider: 2
---

# Einführung in Robot Framework

## 🧪 Keyword-driven Testautomatisierung mit Stil


## Was ist Robot Framework?

- Open-Source Testautomatisierungs-Framework
- Unterstützt Keyword-Driven, Behavior-Driven und Datengetriebene Tests
- Ideal für Akzeptanztests & RPA (Robotic Process Automation)
- Plattformunabhängig (Python-basiert)

## Warum Robot Framework?

- **Lesbarer Code** dank natürlicher Sprache
- Erweiterbar durch Python-Bibliotheken
- Große Community & viele Libraries (z. B. SeleniumLibrary, BrowserLibrary)
- Unterstützt auch API-Tests, Datenbanktests, u. v. m.

## Syntaxbeispiel

```robot
*** Test Cases ***
Beispiel Test
    Öffne Browser    https://example.com    Chrome
    Titel Sollte Sein    Example Domain
    Schließe Browser
```

## Tools & Erweiterungen

RIDE: Robot IDE (GUI-Editor)
VS Code + Robot Framework Language Server für Syntax-Highlighting & IntelliSense
Allure, ReportPortal für erweiterte Reports

## Typische Einsatzgebiete
Web-Testing (z. B. mit Selenium)
REST-API-Tests
RPA (z. B. Formularautomatisierung)
Datenbank-Validierung

## Fazit
Robot Framework = 💡 Lesbare Testsprache trifft auf mächtige Automatisierung

> "Write tests as if writing documentation."

## Kontakt / Fragen?
robotframework.org

GitHub: github.com/robotframework
