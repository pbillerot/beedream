---
title: Texte
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
{{</* texte [mini petite moyenne grande xl] [rouge orange vert cyan bleu pourpre violet marron gris] */>}} ... {{</* /texte */>}}
{{</*centre*/>}} ... {{</*/centre*/>}}
```
<!--more-->
> Pour améliorer la présentation du texte  
Changer la couleur : {{< texte rouge >}}rouge{{< /texte >}} {{< texte orange >}}orange{{< /texte >}} {{< texte vert >}}vert{{< /texte >}} {{< texte cyan >}}cyan{{< /texte >}} {{< texte bleu >}}bleu{{< /texte >}} {{< texte pourpre >}}pourpre{{< /texte >}} {{< texte violet >}}violet{{< /texte >}} {{< texte marron 
>}}marron{{< /texte >}} {{< texte gris >}}gris{{< /texte >}}  
Diminuer ou augmenter la taille de la police : {{< texte mini >}}mini{{< /texte >}} {{< texte petite >}}petite{{< /texte >}} {{< texte moyenne >}}moyenne{{< /texte >}} {{< texte grande >}}grande{{< /texte >}} {{< texte large >}}large{{< /texte >}}  
{{<centre>}}Centrer le texte sur la ligne{{</centre>}}

## Exemple

Le {{< texte orange large >}}Lorem Ipsum{{< /texte >}} est simplement du faux texte employé dans la composition et la mise en page avant impression.

{{<centre>}}{{< texte bleu >}}Le Lorem Ipsum est simplement {{< icone bell >}} du faux texte.{{< /texte >}}{{</centre>}}

```go-html-template
{{</* texte orange large */>}}Le Lorem Ipsum{{</* /texte */>}} est simplement du faux texte employé dans la composition et la mise en page avant impression.

{{</*centre*/>}}{{</* texte bleu */>}}Le Lorem Ipsum est simplement {{</* icone bell */>}} du faux texte.{{</* /texte */>}}{{</*/centre*/>}}
```
- <a href="https://fomantic-ui.com/elements/icon.html" target="_blank">Lien vers la bibliothèque d'icônes</a>