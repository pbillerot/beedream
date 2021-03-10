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
{{</* texte [tiny small medium large huge] [red orange green teal blue purple violet brown grey] */>}} ... {{</* /texte */>}}
{{</*centre*/>}} ... {{</*/centre*/>}}
```
<!--more-->
> Pour améliorer la présentation du texte  
Changer la couleur : {{< texte red >}}red{{< /texte >}} {{< texte orange >}}orange{{< /texte >}} {{< texte green >}}green{{< /texte >}} {{< texte teal >}}teal{{< /texte >}} {{< texte blue >}}blue{{< /texte >}} {{< texte purple >}}purple{{< /texte >}} {{< texte violet >}}violet{{< /texte >}} {{< texte brown 
>}}brown{{< /texte >}} {{< texte grey >}}grey{{< /texte >}}  
Diminuer ou augmenter la taille de la police : {{< texte tiny >}}tiny{{< /texte >}} {{< texte small >}}small{{< /texte >}} {{< texte medium >}}medium{{< /texte >}} {{< texte large >}}large{{< /texte >}} {{< texte huge >}}huge{{< /texte >}}  
{{<centre>}}Centrer le texte sur la ligne{{</centre>}}

## Exemple

Le {{< texte red huge >}}Lorem Ipsum{{< /texte >}} est simplement du faux texte employé dans la composition et la mise en page avant impression.

{{<centre>}}{{< texte blue >}}Le Lorem Ipsum est simplement {{< icone bell >}} du faux texte.{{< /texte >}}{{</centre>}}

```go-html-template
{{</* texte huge */>}}Le Lorem Ipsum{{</* /texte */>}} est simplement du faux texte employé dans la composition et la mise en page avant impression.

{{</*centre*/>}}{{</* texte blue */>}}Le Lorem Ipsum est simplement {{</* icone bell */>}} du faux texte.{{</* /texte */>}}{{</*/centre*/>}}
```
- <a href="https://fomantic-ui.com/elements/icon.html" target="_blank">Lien vers la bibliothèque d'icônes</a>