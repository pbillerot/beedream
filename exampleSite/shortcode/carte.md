---
title: Carte
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
```tpl
{{</* cartes taille="petite moyenne grande large" */>}}
{{</* carte image="image" diapo="diapo" titre="titre" lien="lien" pdf="pdf" taille="..." */>}}
texte...
{{</* /carte */>}}
{{</* /cartes */>}}
```
<!--more-->
> Affichage de cartes pour  
> - agrandir seulement l'image `diapo=`  
> - télécharger le pdf `pdf=`  
> - agrandir l'image et télécharger le pdf `image=` et `pdf=`  
> - ouvrir seulement une page `lien=` et éventuellement télécharger un pdf `pdf=`

{{< cartes taille="petite">}}

{{< carte titre="Hébergement" pdf="/site/media/hebergement.pdf" >}}{{< /carte >}}

{{< carte image="/site/media/markdown.jpg" titre="La syntaxe du Markdown" lien="/markdown/syntax" taille="moyenne" >}}
Markdown est un *langage de balisage léger* dans le but d’offrir une syntaxe facile à lire et à écrire.  
Un document balisé par **Markdown** sera converti en **HTML** avant d'être affiché dans le site web.
{{< /carte >}}

{{< carte image="/site/media/hebergement.jpg" titre="Classement des hébergeurs web VPS" pdf="/site/media/hebergement.pdf" lien="https://www.tophebergeursweb.com/" taille="grande" >}}Les hébergeurs web proposent des offres de serveurs VPS offrant des caractéristiques flexibles et variés. Quelque soit votre projet web, il sera plus intéressant d’acquérir un serveur VPS. Plus puissant, plus performant et plus évolutif les serveurs VPS correspondent aux besoins de chacun. Vous cherchez une solution pour héberger des projets web de grandes tailles alors la solution d’hébergement VPS est faite pour vous. Nous avons analysé et évalué les meilleures offres d’hébergements VPS et nous vous proposons un classement des meilleures hébergeurs VPS.{{< /carte >}}

{{< carte diapo="/site/media/shortcode.svg" titre="Les code courts (shortcodes)" taille="large" >}}{{< /carte >}}

{{< /cartes >}}

---

```tpl
{{</* cartes taille="petite" */>}}

{{</* carte titre="Hébergement" pdf="/site/media/hebergement.pdf" */>}}{{</* /carte */>}}

{{</* carte image="/site/media/markdown.jpg" titre="La syntaxe du Markdown" lien="/markdown/syntax" taille="moyenne" */>}}
Markdown est un *langage de balisage léger* dans le but d’offrir une syntaxe facile à lire et à écrire.  
Un document balisé par **Markdown** sera converti en **HTML** avant d'être affiché dans le site web.
{{</* /carte */>}}

{{</* carte image="/site/media/hebergement.jpg" titre="Classement des hébergeurs web VPS" pdf="/site/media/hebergement.pdf" lien="https://www.tophebergeursweb.com/" taille="grande" */>}}Les hébergeurs web proposent des offres de serveurs VPS offrant des caractéristiques flexibles et variés. Quelque soit votre projet web, il sera plus intéressant d’acquérir un serveur VPS. Plus puissant, plus performant et plus évolutif les serveurs VPS correspondent aux besoins de chacun. Vous cherchez une solution pour héberger des projets web de grandes tailles alors la solution d’hébergement VPS est faite pour vous. Nous avons analysé et évalué les meilleures offres d’hébergements VPS et nous vous proposons un classement des meilleures hébergeurs VPS.{{</* /carte */>}}

{{</* carte diapo="/site/media/shortcode.svg" titre="Les code courts (shortcodes)" taille="large" >}}{{</* /carte */>}}
{{</* /cartes */>}}
```
