---
title: Diaporama
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
{{</* diaporama */>}}
```
<!--more-->
> Diaporama des images d'une page
> Il suffira de placer le code `{{</* diaporama */>}}` dans la page pour visulaiser les images dans un diaporama.

## Exemple

```go-html-template
{{</* diaporama */>}}
{{</* image image="/site/media/default1.jpg" */>}}
{{</* image image="/site/media/default1.jpg" */>}}
```
{{< diaporama >}}

{{< image image="/site/media/default1.jpg" >}}

{{< image image="/site/media/default2.jpg" >}}

