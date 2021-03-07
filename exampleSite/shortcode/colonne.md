---
title: Colonne
draft: false 
date: 2021-02-20 
cover: /shortcode/shortcode.svg
tags:
- shortcode
menu: 
  main:
    parent: shortcode
---
```go-html-template
{{</* colonnes [two, three ]*/>}}
...
<---> saut de colonne
...
{{</* /colonnes */>}}
```

<!--more-->

>Permet de présenter le {{< texte orange >}}texte sur plusieurs colonnes{{< /texte >}}, deux (`two`) par défaut _si la taille de l'écran le permet_. Le saut de colonne sera provoqué par le marqueur `<--->`

## Exemple

{{< colonnes three >}}
Le **Lorem Ipsum** est simplement du faux texte employé dans la composition et la mise en page avant impression.
<--->
Il n'a pas fait que survivre {{< texte red >}}cinq siècles{{< /texte >}}, mais s'est aussi adapté à la bureautique informatique, sans que son contenu n'en soit modifié.
<--->
{{< centre >}}**D'où vient-il {{< texte orange >}}{{< icone question circle >}}{{< /texte >}}**{{< /centre >}}

*Contrairement à une opinion répandue, le Lorem Ipsum n'est pas simplement du texte aléatoire.

Il trouve ses racines dans une oeuvre de la littérature latine classique datant de 45 av. J.-C., le rendant vieux de 2000 ans.*
{{< /colonnes >}}

```go-html-template
{{</* colonnes three */>}}
Le **Lorem Ipsum** est simplement du faux texte employé dans la composition et la mise en page avant impression.
<--->
Il n'a pas fait que survivre {{</* texte red */>}}cinq siècles{{</* /texte */>}}, mais s'est aussi adapté à la bureautique informatique, sans que son contenu n'en soit modifié.
<--->
{{</* centre */>}}**D'où vient-il {{</* texte orange */>}}{{</*icone question circle */>}}{{</*/texte*/>}}**{{</* centre */>}}

*Contrairement à une opinion répandue, le Lorem Ipsum n'est pas simplement du texte aléatoire.

Il trouve ses racines dans une oeuvre de la littérature latine classique datant de 45 av. J.-C., le rendant vieux de 2000 ans.*
{{</* /colonnes */>}}
```
