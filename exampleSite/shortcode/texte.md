---
title: Texte
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
```go-html-template
{{</* texte [xs s m l xl] [rouge orange vert cyan bleu pourpre violet marron gris] */>}} ... {{</* /texte */>}}
{{</*centre*/>}} ... {{</*/centre*/>}}
```
<!--more-->

> Pour améliorer la présentation du texte  
Changer la couleur : {{< texte rouge >}}rouge{{< /texte >}} {{< texte orange >}}orange{{< /texte >}} {{< texte vert >}}vert{{< /texte >}} {{< texte cyan >}}cyan{{< /texte >}} {{< texte bleu >}}bleu{{< /texte >}} {{< texte pourpre >}}pourpre{{< /texte >}} {{< texte violet >}}violet{{< /texte >}} {{< texte marron 
>}}marron{{< /texte >}} {{< texte gris >}}gris{{< /texte >}}  
Diminuer ou augmenter la taille de la police : {{< texte xs >}}extra short{{< /texte >}} {{< texte s >}}short{{< /texte >}} {{< texte m >}}moyenne{{< /texte >}} {{< texte l >}}large{{< /texte >}} {{< texte xl >}}extra large{{< /texte >}}  
{{<centre>}}Centrer le **texte** sur la ligne{{</centre>}}

## Exemple

Le {{< texte orange l >}}Lorem Ipsum{{< /texte >}} est simplement du faux texte employé dans la composition et la mise en page avant impression.

{{<centre>}}{{< texte bleu m >}}Le Lorem Ipsum **est** simplement {{< icone bell >}} du faux texte.{{< /texte >}}{{</centre>}}

```go-html-template
{{</* texte orange l */>}}Le Lorem Ipsum{{</* /texte */>}} est simplement du faux texte employé dans la composition et la mise en page avant impression.

{{</*centre*/>}}{{</* texte bleu l */>}}Le Lorem Ipsum **est** simplement {{</* icone bell */>}} du faux texte.{{</* /texte */>}}{{</*/centre*/>}}
```
- <a href="https://fomantic-ui.com/elements/icon.html" target="_blank">Lien vers la bibliothèque d'icônes</a>