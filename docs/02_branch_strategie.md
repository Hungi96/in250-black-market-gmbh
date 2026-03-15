# Branching Strategie

## Überblick

Damit im Repository strukturiert gearbeitet werden kann und Änderungen nicht direkt im `main` Branch landen, verwenden wir eine einfache Branching Strategie nach dem Prinzip von **GitHub Flow**.

Der `main` Branch enthält immer eine stabile und funktionierende Version des Projekts. Änderungen werden daher nicht direkt im `main` Branch gemacht, sondern zuerst in eigenen Feature-Branches entwickelt.

So bleibt der Hauptbranch stabil und Änderungen können über Pull Requests überprüft werden, bevor sie in den `main` Branch übernommen werden.

## Workflow

Der typische Ablauf bei Änderungen im Projekt sieht wie folgt aus:

1. Zuerst wird der aktuelle Stand vom `main` Branch geholt
2. Danach wird ein neuer Feature-Branch erstellt
3. Die Änderungen werden im Feature-Branch entwickelt
4. Änderungen werden regelmässig committet und auf GitHub gepusht
5. Anschliessend wird ein Pull Request erstellt
6. Die Änderungen werden überprüft
7. Der Pull Request wird in den `main` Branch gemerged

Durch diesen Ablauf bleibt der `main` Branch immer stabil und Änderungen sind gut nachvollziehbar.

## Branch Namenskonvention

Damit klar ist, wofür ein Branch gedacht ist, werden Branches nach einem einfachen Schema benannt:

feat/<feature-name>  
fix/<bug-name>  
docs/<documentation>

Beispiele:

feat/login-feature  
fix/navigation-bug  
docs/update-readme  

So kann man sofort erkennen, welche Art von Änderung in einem Branch gemacht wurde.

## Vorteile dieser Strategie

Diese Strategie hat mehrere Vorteile:

- klare Struktur im Repository  
- stabile Version im `main` Branch  
- Änderungen sind über Pull Requests nachvollziehbar  
- bessere Zusammenarbeit im Team  

## Releases

Wenn eine stabile Version erreicht ist, wird diese mit einem **Git Tag** markiert.

Beispiel:

v1.0

Damit ist sofort sichtbar, welche Version des Projekts veröffentlicht wurde.