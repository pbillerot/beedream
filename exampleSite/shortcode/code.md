---
title: Code
draft: false 
date: 2021-02-20 
cover: /site/media/shortcode.svg
tags:
- shortcode
# Ne sera par affiché dans le sommaire
_build:
   list: false
menu: 
  page:
    parent: shortcode

style: bee-doc
---
```tpl
{{</* code "fichier.ext" "langage" */>}}
```
<!--more-->
> Insertion dans le document d'un code source

## Exemple

{{< code "/site/config.yaml" "yaml" >}}

```tpl
{{</* code "/site/config.yaml" "yaml" */>}}
```
