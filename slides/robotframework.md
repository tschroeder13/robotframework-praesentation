---
marp: true
theme: rose-pine-moon
paginate: true
headingDivider: 2
---


# Robot Framework Appetizer
<script type="text/javascript" src="/path/to/highlight.pack.js"></script>
<script type="text/javascript" src="/path/to/highlightjs-robot/robot.js"></script>
<script type="text/javascript">
    hljs.registerLanguage('robot', window.hljsDefineRobot);
    hljs.highlightAll();
</script>

![bg right fit](https://github.com/tschroeder13/robotframework-praesentation/raw/main/slides/RF-Logo.png)

<!-- 
Motivation: Bedarf an LDAP Bibliothek zum testen i.R. einer IDM Lösung
 -->

## Was ist Robot Framework?
- Open-Source RPA & Testautomatisierungs-Framework
- Unterstützt v.a. Keyword-Driven und Datengetriebene Tests aber auch BDD
- Ideal für Akzeptanztests & RPA (Robotic Process Automation)
- Plattformunabhängig (Python-basiert)
- Breite Unterstützung durch die [Robot Framework Foundation](https://robotframework.org/foundation/)


<!--
RPA: Robotic Process Automation
-->

<!-- footer: "[BDD](https://docs.robotframework.org/docs/testcase_styles/bdd), [DDT](https://docs.robotframework.org/docs/testcase_styles/datadriven)" -->

## Warum Robot Framework?

- **Lesbarer Code** dank natürlicher Sprache - nicht nur Englisch
- Erweiterbar durch Bibliotheken in verschiedenen Programmiersprachen
- Große Community & viele Libraries (z. B. SeleniumLibrary, BrowserLibrary, u.v.m.)
- Unterstützt auch API-Tests, Datenbanktests, **LDAP Tests** u. v. m.

<!-- footer: "" -->

## Syntaxbeispiel

```robot
*** Settings ***
Library    Browser

*** Variables ***
${BROWSER}    chromium
${HEADLESS}    false

*** Test Cases ***
Create Quote for Car
    Open Insurance Application
    Enter Vehicle Data for Automobile
    Enter Insurant Data
    Enter Product Data
    Select Price Option
    Send Quote
    End Test

*** Keywords ***
Open Insurance Application
    New Browser    browser=${BROWSER}    headless=${HEADLESS}
    New Context    locale=en-GB
    New Page    http://sampleapp.tricentis.com/

Enter Vehicle Data for Automobile
    Click    div.main-navigation >> "Automobile"
    Select Options By    id=make    text    Audi
    Fill Text    id=engineperformance    110
    Fill Text    id=dateofmanufacture    06/12/1980
    Select Options By    id=numberofseats    text    5
    Select Options By    id=fuel    text    Petrol    
    Fill Text    id=listprice    30000
    Fill Text    id=licenseplatenumber    DMK1234
    Fill Text    id=annualmileage   10000 
    Click    section[style="display: block;"] >> text=Next »
    [...]
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

> Write tests as if writing documentation.

## Links / Kontakte / Fragen?
[robotframework.org](https://robotframework.org/)

GitHub: github.com/robotframework

[Repository zu Many Kasirihas Talk auf der Robocon 2022](https://github.com/manykarim/robocon-fortheveryfirsttime)