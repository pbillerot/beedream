---
title: Répertoire
draft: false 
date: 2021-02-20 
cover: /site/media/shortcode.svg
tags:
- shortcode
# Ne sera par affiché dans le sommaire
_build:
   list: false
style: bee-doc
menu: 
  page:
    parent: shortcode
---
```tpl
{{</* repertoire "répertoire" */>}}
```
<!--more-->
> Affichage des fichiers présents dans le `répertoire`  

## Exemple

### répertoire
```
├── fichiers
│   ├── Batterie 110.wav
│   ├── bee.svg
│   ├── config.yaml
│   ├── config.zip
│   ├── document.doc
│   ├── document.docx
│   ├── document.odt
│   ├── Neil Young - Heart Of Gold.mp3
│   ├── paper.jpg
│   ├── pdf.pdf
│   ├── presentation.odp
│   ├── presentation.ppt
│   ├── presentation.pptx
│   ├── tableur.ods
│   ├── tableur.xls
│   ├── tableur.xlsx
│   └── walking.gif
└── index.md
```
### index.md
```tpl
{{</* repertoire "/shortcode/fichiers" */>}}
```
### résultat
{{< repertoire "/shortcode/fichiers" >}}

