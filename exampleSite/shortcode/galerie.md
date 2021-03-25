---
title: Galerie
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
{{</* galerie repertoire /*/>}} ou
{{</* galerie */>}}
{{</* galet image="image" [lien="lien"] */>}}
{{</* /Galerie */>}}
```
<!--more-->
> Affichages des images trouvées dans le `repertoire`  
> Présentation en plusieurs colonnes en fonction de la taille de l'écran et de l'espace vertical disponible un peu comme un maçon installant des pierres dans un mur.  
> Galerie de galets (images) avec lien possible vers une page ou un site.  
> La taille des images et le nombre de colonnes varieront en fonction de la taille de l'écran.

## Exemple 1

```go-html-template
{{</* galerie "/site/media" /*/>}}
```
{{< galerie "/site/media" />}}

## Exemple 2

```go-html-template
{{</* galerie */>}}
{{</* galet image="/site/media/deploiement.png" */>}}
{{</* galet image="/site/media/markdown.jpg" */>}}
{{</* galet image="/site/media/shortcode.svg" */>}}
{{</* galet image="/site/media/default2.jpg" */>}}
{{</* /galerie */>}}
```
{{< galerie >}}
{{< galet image="/site/media/deploiement.png" >}}
{{< galet image="/site/media/markdown.jpg" >}}
{{< galet image="/site/media/shortcode.svg" >}}
{{< galet image="/site/media/default2.jpg" >}}
{{< /galerie >}}
