---
title: Label
draft: false 
date: 2021-02-20 
cover: /site/media/shortcode.svg
style: bee-doc
tags:
- shortcode
# Ne sera par affiché dans le sommaire
_build:
   list: false
menu: 
  page:
    parent: shortcode

---
```tpl
{{</* label label="libellé" [icone=""] [lien="lien"] */>}}
```
<!--more-->
> Affichage d'un bouton actif ou non  

> {{< icone arrow circle right >}} <a href="https://semantic-ui.com/elements/icon.html" target="_blank">Lien vers la bibliothèque d'icônes</a>


## Exemple

{{< label label="01 02 03 04 05" icone="phone" >}}
{{< label label="abeille@laruche.com" icone="mail" lien="mailto:abeille@laruche.com">}}

```tpl
{{</* label label="01 02 03 04 05" icone="phone" */>}}
{{</* label label="abeille@laruche.com" icone="mail" lien="mailto:abeille@laruche.com" */>}}
```
