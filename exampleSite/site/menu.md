---
title: "Les Menus"
date: 2021-03-08
draft: false
tags:
- menu
- contenu
cover: "/site/media/menu.svg"
style: bee-doc
menu:
  page:
    parent: site
    weight: 40
---
<!--more-->
{{< image image="/site/captures/captures-menu.png" position="droite" taille="m" >}}
>4 menus seront paramétrables dans le thème Beedream :

{{< toc >}}

## 1 - Menu de navigation
>La barre de `navigation` de haut d'écran sera décrite exclusivement dans le fichier de configuration du site `/site/config.yaml`  
À réserver pour des liens vers des sites externes  
Le lien sera ouvert dans un autre onglet  
Le nom de l'icône sera déclarée par le paramètre `pre`

> <a href="https://fomantic-ui.com/elements/icon.html" target="_blank">{{< icone external alternate >}} Lien vers la bibliothèque d'icônes</a>

*À noter que l'ordre de présentation des items de menu sera trié d'abord sur la propriété `weight` et ensuite dans l'ordre alphabétique.*

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

## 2 - Menu des pages de contenu

> Ce menu sera défini au niveau des méta-données de chaque page

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
    weight: 1 # tri
```
Pour cet exemple, le menu **Markdown** va pointer directement sur la page.
Il ne possèdera pas de sous-menu

### Menu avec sous-menu
{{< image image="/site/captures/capture-menu-accordeon.png" position="droite"  taille="m">}}
> Ce type de menu sera présenté sous forme d'accordéon

Dans un 1er temps il faudra définir le titre du menu dans un fichier `_index.md` ou en le déclarant dans `config.yaml` comme les autres menus.

Exemple en déclarant le titre du menu dans `/site/config.yaml`
```yaml
menu: 
  page:
  - name: "Shortcodes"
    identifier: shortcode
    weight: 2
```

Exemple dans `/shortcodes/_index.md` l'identifiant `shortcode` sera utilisé pour raccrocher les items à ce menu.
```yaml
---
title: Shortcodes
draft: false 
menu: 
  page:
    identifier: shortcode
    weight: 2
---
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

## 3 - Menu des liens
> Le menu `links` sera plus réservé pour des pages internes générales au site du genre "A propos", "Informations légales", etc.  
Il pourra être décrit dans le fichier de configuration du site `/site/config.yaml`

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

mais aussi directement dans les méta-données de la page comme suit :

```yaml
---
title: "Todo"
date: 2021-03-08
draft: false
_build:
   list: false
cover: "/site/media/todo.png"
# Déclaration de la page dans le menu links
menu:
   links:
      weight: 10
---
```

## 4 - Menu des News
> Le menu `news` sera le menu des pages évènementielles, les têtes de gondole", les pages à mettre en évidence...

L'inscription d'une page à ce menu se fera via la `categorie` **news** dans les metadonnées de la page.

```yaml
---
title: "Quoi de neuf dans Beedream"
date: 2021-03-11
draft: false
tags:
categories:
- news
---
```
