---
title: [[scholarium.at]]-Inhalte als [[digital garden]]
---

## Ausgehend von FAQ, mit allen Inhalten als Antworten auf Fragen
### Beginnend bei "Was ist das scholarium?"

### [[Questions vs claims as titles]]: Claims besser?
:PROPERTIES:
:ID:db2ede2d-0f1c-4a6b-ae7d-65c16b1e5b9f
:END:

## [[Differenzierung freie Inhalte und premium-Inhalte]]

## Videos als didaktische Ergänzung zu Karten - Erklärung einzelner Argumente/Konzepte/Quellen
:PROPERTIES:
:ID:0dace106-1bf3-4be3-af07-6657b38eddc3
:END:
### alle Videos müssten dann unlisted auf Youtube gehostet werden

### youtube-embed-code von Roam wird direkt in md-File geschrieben, aber kein Markdown - benötigt also script, um in gatsby angezeigt zu werden

### ersetzt [[online courses]]?

## Schon vorhandene Inhalte: 
### Inhalte aus Scholien und Büchern, aufspalten und verlinken

### Aufzeichnungen? als Quellen?

### sources & quotes aus [[zotero]], geordnet nach Themen (zu Fragen?)

## Fragen
### {DONE}} Versionen nutzbar für [Mehrsprachigkeit]([[Mehrsprachige Ideenkollaboration - Multilingual collaboration on ideas]])? 
#### derzeit noch nicht, da Versionen nicht exportiert werden
##### es wird immer die gerade ausgewählte Version exportiert, dazu

## Umsetzung
:PROPERTIES:
:ID:dc4dc4f9-eae1-48d9-bb5a-f7098ed32292
:END:
### ~~ wordpress eher schlecht geeignet dafür ~~
#### API calls and flat files through GraphQL, and builds the static site based on configuration settings

#### Files are directly delivered from the server without rendering (?) to visitors

#### https://kinsta.com/de/blog/gatsby-wordpress/ a good hint for a possible solution;

#### Access all WordPress data using GraphQL queries
##### GraphQL is the key to solve this problem; https://www.wpgraphql.com/

#### Main problem will be the security restrictions on WPengine Servers;
##### headless wp pages are possible with wpengine

##### can you run a static and a dynamic version of your wp-website?

### Inhalte erstellen und bearbeiten in [[Roam]]
#### erste Version in https://roamresearch.com/#/app/Studium-scholarium/page/_xhvEzwcF

### Django-userAuth nutzen für Zugangskontrolle zu statischem Ordner
:PROPERTIES:
:ID:e924f968-4c46-4b94-be0c-4358a60e1e7b
:END:
#### You'd probably have to use Django's router to map to all of the html files in the Gatsby build directory.

### gatsby-digital garden: https://github.com/mathieudutour/gatsby-digital-garden
#### enthält Html, generiert aus Markdown-Dateien von Roam-Export
##### [[Gatsby]] empfiehlt [[MDX]], für volle Funktionalität
###### MD funktioniert jedoch auch problemlos

#### Gatsby Documentation: https://www.gatsbyjs.org/docs/
##### Setup Gatsby:
###### brew install npm

###### npm install -g gatsby-cli

###### gatsby new gatsby-site-name source

###### gatsby-config.js legt unter "root-note" die Homepage fest

##### Gatsby Development Server
###### cd gatsby-site-name

###### gatsby develop

###### http://localhost:8000

##### Gatsby Production
###### cd gatsby-site-name

###### gatsby build

###### gatsby serve

#### Funktionsweise der Export-Automatisierung:
##### scraping mit puppeteer für Automatisierung

#### Probleme:
##### Block embedding funktioniert nicht

##### "ToDos"/"Checkboxen" werden standardmäßig nicht angezeigt bzw. als funktionsloser Code

##### [[Aliases]] funktionieren nicht, bräuchten zusätzliches Script - in [[Roam]] sind interne Links stets wiki-links 

##### Notizen/Pages mit Leerzeichen werden unter Umständen nicht angezeigt wie z. B. [Mehrsprachige Ideenkollaboration/Multilingual collaboration on ideas], da Leerzeichen durch ein "-" ersetzt werden
###### Schrägstrich ist wohl eher das Problem

##### lose Notizen werden nicht angezeit
###### Notizen existieren nur im Netzwerk/Verbindung zueinander

##### Die Relevanz einer Notiz lässt sich nicht darstellen
###### u. U. findet man besonders wichtige Notizen erst nach mehreren Klick

##### Wenn Filename ungleich angezeigter Name ist, dann gibt es einen Error:
###### [Wiener Schule]([[[Was ist die Wiener Schule?]]](http://localhost:9000/example-dir/Was%20ist%20die%20Wiener%20Schule?))

###### Er sucht "Was ist die Wiener Schule", obwohl das File "Wiener Schule" heißt.

### Alternativen
#### alternativ zu gatsby lässt sich auch [[jekyll]] verwenden

#### https://www.cloak.ist/roam (5$/Monat)

#### ev. später Einlesen eines private Graph über API
##### Studenten als editors

#### oder Hinzufügen von Unterstützern als Readers & Editors über API
