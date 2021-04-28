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

```tpl
{{</* repertoire "/shortcode/fichiers" */>}}
```
### résultat
{{< repertoire "/shortcode/fichiers" >}}

