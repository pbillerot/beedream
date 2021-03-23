---
title: "Menu"
date: 2021-03-08
draft: false
tags:
- technique
cover: "/site/media/menu.svg"
style: bee-doc
menu:
  page:
    weight: 3
---
<!--more-->
{{< image image="/site/captures/captures-menu.jpg" position="droite" taille="m" >}}
>3 menus seront paramétrables dans le thème Beedream :

1. le [menu de navigation](#menu_navigation) en haut de la page
1. le [menu des liens](#menu_liens) dans le bas du sommaire
1. le [menu des pages de contenu](#menu_pages) qui va se présenter au centre de la carte sommaire

<a name="menu_navigation"></a>

## Menu de navigation
>Le menu `navigation` sera décrit dans le fichier de configuration du site `/site/config.yaml`  
À réserver pour des liens vers des sites externes  
Le lien sera ouvert dans un autre onglet

*À noter que l'ordre des présentation des items de menu sera trié d'abord sur la propriété `weight` et ensuite sur l'ordre alphabétique.*

```yaml
menu:
  # menu liens en haut de la page
  # le lien sera ouvert dans un autre onglet
  navigation:  
  - name: "Documentation sur le thème BeeDream"
    url: "https://beedream.billerot.eu/"
    weight: 10
    pre: "help" # nom de l'icône de la bibliothèque des icônes
  - name: "Bibliothèque des icônes"
    url: "https://fontawesome.com/icons?d=gallery&p=2&m=free"
    weight: 20 # pour trier le menu
    pre: "font awesome flag" # nom de l'icône de la bibliothèque des icônes
  - name: "Documentation Hugo"
    url: "https://gohugo.io/"
    weight: 30 # pour trier le menu
    pre: "hospital symbol" # nom de l'icône de la bibliothèque des icônes
```
<a name="menu_liens"></a>

## Menu des liens
> Le menu `links` sera réservé pour des pages générales au site du genre "A propos", "Informations légales", etc.  
Il sera décrit dans le fichier de configuration du site `/site/config.yaml`

```yaml
menu:
  # menu qui va apparaître en bas de la carte du sommaire
  # le lien sera ouvert dans l'onglet courant
  # à réserver pour des liens vers des pages du site
  links: 
  - name: "README"
    url: "/site/readme/"
    weight: 10 # pour trier le menu
  - name: "TODO"
    url: "/site/todo/"
    weight: 20 # pour trier le menu
```

<a name="menu_pages"></a>

## Menu des pages de contenu
> Ce menu sera défini au niveau de l'entête de chaque page

### Menu simple:
```yaml
title: Markdown
draft: false 
date: 2021-02-23
tags:
- markdown
cover: /site/media/markdown.jpg
menu:
  page:
    weight: 2 # tri
```
Pour cet exemple, le menu **Markdown** va apparaître et pointer directement sur la page.
Il ne possèdera pas de sous-menu

### Menu avec sous-menu
{{< image image="/site/captures/capture-menu-accordeon.jpg" position="droite"  taille="m">}}
> Ce type de menu sera présenté sous forme d'accordéon

Dans un 1er temps il faudra définir le titre du menu dans un fichier `_index.md` ou en le déclarant dans `config.yaml` comme les autres menus.

Exemple dans `/shortcodes/_index.md` l'identifiant `shortcode` sera utilisé pour raccrocher les items à ce menu.
```yaml
title: Shortcodes
draft: false 
menu: 
  page:
    identifier: shortcode
    weight: 3
```
Un item du menu sera défini directement dans la page en précisant le `parent` du menu   
Exemple avec `/shortcodes/carte.md`
```yaml
title: Carte
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
```
