---
title: type of block or page
---

## Müssen Kartentypen festgelegt werden?

## Vorschlag für Typen:
### Topic: Thematische Übersichtskarte
#### Ist eine geordnete Sammlung/Outline von Zetteln

### Source: Quelle
#### ISBN, ISSN, URL

### quote?

### Note/Draft/Comment: für alle Zettel, die noch nicht "evergreen" sind

### Claim/Question/Answer: [[evergreen notes]]

### Evidence

### [[tools]]

## Kartentypen im Gegensatz zu unterschiedslosen Bullet points (Roam) und Files (Obsidian, Foam)

## Vorteile:
### Regt eine Disziplin mit didaktischem Nutzen an
#### Leitet Workflow an
##### von notes/drafts zu evergreen

##### von source zu quotes und weiter mit note- oder claim/evidence-Zettel, die auf quotes verweisen

### Bietet Normen für größere Übersichtlichkeit und gegenseitige Relevanz

### Strukturiert den Diskurs und legt den Fokus auf gute Argumentation

## Nachteile:
### schwer mit Markdown-Files abzubilden
#### mit [[tag]] und [[Ordner]] machbar

### Korsett für Gedanken, das Schwelle zum Schreiben und Transaktionskosten der Kollaboration erhöht

## "Kategorien" anlegen und farblich kennzeichnen mit folgendem Code: data-tag muss angepasst werden!
### ```css


/* Custom data tags */
span.rm-page-ref[data-tag="TwitterPost"] {
    background: #81D5ED !important;
    color: white !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Literature Notes"] {
    background: #9769FF !important;
    color: white !important;
    padding: 3px 7px;
    font-weight: 500;
    line-height: 2em;
}


span.rm-page-ref[data-tag="Evergreens"] {
    background: #0DBAC6 !important;
    color: #fff !important;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Seedling"] {
    color: #0dbac6 !important;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"] {
    color: #FCB815 !important;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"]:before {
    content: '✦ '
}

span.rm-page-ref[data-tag="Illustrated Notes"] {
    color: #7172FC;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Garden Notes"] {
    color: #9DBC13;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Video Tutorial"] {
    color: #db3b8d;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Essay"] {
    background: #ADCB2A;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Livestream"] {
    color: #B979CF;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Talk"] {
    background: #7172FC;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Waiting"] {
    background: #F9C866;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Researching"] {
    background: #FF9D66 !important;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Synthesising"] {
    background: #FC766F !important;
    color: #fff !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Alive"] {
    background: #EE5F85 !important;
    color: #fff !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}
```
