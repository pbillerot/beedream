---
title: Icône
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
---

```go-html-template
{{</* icone nomIcone */>}}
```
<!--more-->
> Pour afficher une **icône** dans le texte  
Le nom de l'icône sera à piocher dans la [bibliothèque d'icônes](https://fomantic-ui.com/elements/icon.html)

## Exemple

Le **Lorem Ipsum** est simplement du faux {{< icone bell >}} texte employé dans la composition et la mise en page avant impression.

```go-html-template
Le **Lorem Ipsum** est simplement du faux {{</* icone bell */>}} texte employé dans la composition et la mise en page avant impression.
```
