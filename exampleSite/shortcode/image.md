---
title: Image
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
{{</* image image="image" titre="légende" lien="lien" position="gauche droite" taille="mini petite moyenne grande" */>}}
```
<!--more-->
> Affiche d'une image avec le texte qui l'entoure à droite ou à gauche.  
> Si la position est non renseignée, l'image sera seule sur la ligne 

## Exemple
Contrairement à une opinion répandue, le Lorem Ipsum n'est pas simplement du texte aléatoire. Il trouve ses racines dans une oeuvre de la littérature latine classique datant de 45 av. J.-C., le rendant vieux de 2000 ans.
{{< image image="https://fomantic-ui.com/images/wireframe/image.png" titre="Légende de l'image" lien="lien" position="droite" taille="petite" >}} 
On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

{{< image image="https://fomantic-ui.com/images/wireframe/image.png" titre="mini" taille="mini" >}} 
{{< image image="https://fomantic-ui.com/images/wireframe/image.png" titre="petite" taille="petite" >}} 
{{< image image="https://fomantic-ui.com/images/wireframe/image.png" titre="moyenne" taille="moyenne" >}} 
{{< image image="https://fomantic-ui.com/images/wireframe/image.png" titre="grande" taille="grande" >}} 

```go-html-template
Contrairement à une opinion répandue, le Lorem Ipsum n'est pas simplement du texte aléatoire. Il trouve ses racines dans une oeuvre de la littérature latine classique datant de 45 av. J.-C., le rendant vieux de 2000 ans.
{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" titre="Légende de l'image" lien="lien" position="droite" taille="petite" */>}} 
On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" titre="mini" taille="mini" */>}} 
{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" titre="petite" taille="petite" */>}} 
{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" titre="moyenne" taille="moyenne" */>}} 
{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" titre="grande" taille="grande" */>}} 
```
