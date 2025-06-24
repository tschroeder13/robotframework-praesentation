---
marp: true
theme: rose-pine-moon
paginate: true
headingDivider: 2
---

# Einführung in Robot Framework

## 🧪 Keyword-driven Testautomatisierung mit Stil

## Was ist Robot Framework?

- Open-Source RPQ & Testautomatisierungs-Framework
- Unterstützt Keyword-Driven, Behavior-Driven und Datengetriebene Tests
- Ideal für Akzeptanztests & RPA (Robotic Process Automation)
- Plattformunabhängig (Python-basiert)
- Breite Unterstützung durch die [Robot Framework Foundateion](https://robotframework.org/foundation/)

## Warum Robot Framework?

- **Lesbarer Code** dank natürlicher Sprache - nicht nur Englisch
- Erweiterbar durch Bibliotheken in verschiedenen Programmiersprachen
- Große Community & viele Libraries (z. B. SeleniumLibrary, BrowserLibrary)
- Unterstützt auch API-Tests, Datenbanktests, LDAP Tests u. v. m.

## Syntaxbeispiel

```robot
*** Test Cases ***
Beispiel Test
    Öffne Browser    https://example.com    Chrome
    Titel Sollte Sein    Example Domain
    Schließe Browser
```

## Tools & Erweiterungen
VS Code + Robot Framework Plugin
[Robot Framework AIO](https://robotframework-aio.org/)
RIDE: Robot IDE (GUI-Editor)
Allure, ReportPortal für erweiterte Reports
Integration in ALM und CI Pipelines

## Typische Einsatzgebiete
Web-Testing (z. B. mit Selenium)
REST-API-Tests
RPA (z. B. Formularautomatisierung)
Datenbank-Validierung

## Library erstellen
Implementierung in Python
Unit Testing mit pytest oder unittest
Akzeptanztests mit Robot Framework und der Implementierung
Dokumentation Generator (robot-libdoc)
Abhängigkeiten verwalten, packen und veröffentlichen mit Poetry
Lokale Aufgabenautomation   



## Fazit
Robot Framework = 💡 Lesbare Testsprache trifft auf mächtige Automatisierung

> "Write tests as if writing documentation."

## Links / Kontakte / Fragen?
[robotframework.org](https://robotframework.org/)

GitHub: github.com/robotframework
[Repository zu Many Kasirihas Talk auf der Robocon 2022](https://github.com/manykarim/robocon-fortheveryfirsttime)