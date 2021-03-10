---
title: Icône
draft: false 
date: 2021-02-20 
cover: /site/media/shortcode.svg
# Ne sera par affiché dans le sommaire
_build:
   list: false
menu: 
  main:
    parent: shortcode
---

```go-html-template
{{</* icone nomIcone */>}}

```
<!--more-->
> Pour afficher une **icône** dans le texte

> {{< icone arrow circle right >}} <a href="https://fomantic-ui.com/elements/icon.html" target="_blank">Lien vers la bibliothèque d'icônes</a>


## Exemple

Le **Lorem Ipsum** est simplement du faux {{< icone bell >}} texte employé dans la composition et la mise en page avant impression.

```go-html-template
Le **Lorem Ipsum** est simplement du faux {{</* icone bell */>}} texte employé dans la composition et la mise en page avant impression.
```
