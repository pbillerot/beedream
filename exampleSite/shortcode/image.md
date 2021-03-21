---
title: Image
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
{{</* image image="image" [lien="lien"] [position="gauche droite"] [taille="s m l xl"] [forme="ronde"] */>}}
```
<!--more-->
> Affiche d'une image avec le texte qui l'entoure à droite ou à gauche.  
> Si la position est non renseignée, l'image sera seule sur sa ligne.  
> Taille {{<texte rouge>}}s{{</texte>}}hort {{<texte rouge>}}m{{</texte>}}edium {{<texte rouge>}}l{{</texte>}}arge e{{<texte rouge>}}x{{</texte>}}xtra-{{<texte rouge>}}l{{</texte>}}arge ou **taille réelle** si le paramètre n'est pas renseignée.  
> La forme de l'image peut être arrondie (*cercle* ou *ovale* en fonction du rapport entre la largeur et la hauteur de l'image).
> 

## Exemple
Contrairement à une opinion répandue, le Lorem Ipsum n'est pas simplement du texte aléatoire. Il trouve ses racines dans une oeuvre de la littérature latine classique datant de 45 av. J.-C., le rendant vieux de 2000 ans.
{{< image image="https://fomantic-ui.com/images/wireframe/image.png" lien="https://fomantic-ui.com/images/wireframe/image.png" position="droite" taille="m" forme="ronde" >}} 
On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

{{< image image="https://fomantic-ui.com/images/wireframe/image.png" taille="s" >}} `taille="s"` (short)  
{{< image image="https://fomantic-ui.com/images/wireframe/image.png" taille="m" >}} `taille="m"` (medium)  
{{< image image="https://fomantic-ui.com/images/wireframe/image.png" taille="l" >}} `taille="l"` (large)  
{{< image image="https://fomantic-ui.com/images/wireframe/image.png" taille="xl" >}} `taille="xl"` (extra large) 
{{< image image="https://fomantic-ui.com/images/wireframe/image.png" >}} taille non précisée 

```go-html-template
Contrairement à une opinion répandue, le Lorem Ipsum n'est pas simplement du texte aléatoire. Il trouve ses racines dans une oeuvre de la littérature latine classique datant de 45 av. J.-C., le rendant vieux de 2000 ans.
{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" lien="https://fomantic-ui.com/images/wireframe/image.png" position="droite" taille="m" forme="ronde" */>}} 
On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

On sait depuis longtemps que travailler avec du texte lisible et contenant du sens est source de distractions, et empêche de se concentrer sur la mise en page elle-même.

{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" taille="s" */>}}..
{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" taille="m" */>}}.. 
{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" taille="l" */>}}..
{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" taille="xl" */>}} 
{{</* image image="https://fomantic-ui.com/images/wireframe/image.png" */>}} 
```
