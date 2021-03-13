---
title: Diaporama
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
{{</* diaporama */>}}
{{</* Galerie [repertoire] */>}}
```
<!--more-->
> Diaporama des images d'une galerie  
> Il suffira de placer le code `{{</* diaporama */>}}` dans la page pour visulaiser les images dans un diaporama.

## Exemple

```go-html-template
{{</* diaporama */>}}
{{</* galerie */>}}
{{</* galet image="/site/media/deploiement.png" */>}}
{{</* galet image="/site/media/markdown.jpg" */>}}
{{</* galet image="/site/media/shortcode.svg" */>}}
{{</* galet image="/site/media/default2.jpg" */>}}
{{</* /galerie */>}}
```
{{< diaporama >}}
{{< galerie >}}
{{< galet image="/site/media/deploiement.png" >}}
{{< galet image="/site/media/markdown.jpg" >}}
{{< galet image="/site/media/shortcode.svg" >}}
{{< galet image="/site/media/default2.jpg" >}}
{{< /galerie >}}
