---
title: Players
draft: false 
date: 2021-02-20 
cover: /site/media/shortcode.svg
tags:
- shortcode
# Ne sera par affiché dans le sommaire
_build:
   list: false
menu: 
  main:
    parent: shortcode
---
```tpl
{{</* players répertoire */>}}
```
<!--more-->
> Affichage des players correspondants aux morceaux de musique présents dans le `répertoire`  
> Seuls les fichiers avec les extensions `.wav` `.ogg` `.mp3` seront proposés.

## Exemple

{{< players "/site/media" >}}

```tpl
{{</* players /site/media */>}}
```
