---
title: Bouton
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
{{</* bouton icone="nom icone" image="image" titre="titre" lien="lien" */>}}
```
<!--more-->

{{< bouton icone="github" image="/site/media/hugo-logo.png" titre="Documentation HUGO" lien="https://gohugo.io/" >}}
{{< bouton icone="github" titre="Sources sur Github" lien="https://github.com/pbillerot/beedream" >}}

```go-html-template
{{</* bouton image="/site/media/hugo-logo.png" titre="Documentation HUGO" lien="https://gohugo.io/" */>}}
{{</* bouton icone="github" titre="Sources sur Github" lien="https://github.com/pbillerot/beedream" */>}}
```
- <a href="https://fomantic-ui.com/elements/icon.html" target="_blank">Lien vers la bibliothèque d'icônes</a>
