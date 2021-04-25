---
title: Galerie
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

```go-html-template
{{</* galerie [sous-repertoire] /*/>}} ou
```
<!--more-->
> Affichages des images trouvées dans le `sous-repertoire` précisé ou dans le répertoire courant  
> Présentation en plusieurs colonnes en fonction de la taille de l'écran et de l'espace vertical disponible un peu comme un maçon installant des pierres dans un mur.  
> La taille des images et le nombre de colonnes varieront en fonction de la taille de l'écran.

> Seul un document `index.md` peut utiliser le shortcode galerie.

## Exemple 1

```go-html-template
{{</* galerie "images" */>}}
```
{{< galerie "images" >}}

