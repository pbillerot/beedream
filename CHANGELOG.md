---
title: "Quoi de neuf dans Beedream ?"
# cd exampleSite/site
# ln -s ../../CHANGELOG.md CHANGELOG.md
date: 2021-03-11
draft: false
tags:
categories:
- news
# Ne sera pas affiché dans le sommaire
_build:
   list: false
---
<!--more-->

À VENIR
-------
- bug shortcode texte dans colonnes qui créé <p>...</p>

1.4.2 du 1er juillet 2021
----------------------
- `fixed` oubli utilisation de la variable .Site.GoogleAnalytics

1.4.2 du 1er juillet 2021
----------------------
- `fixed` implémentation Google Analytics - correction balise

1.4.0 du 1er juillet 2021
----------------------
- `added` implémentation Google Analytics v4

1.3.17 du 25 juin 2021
----------------------
- `removed` debug rendre-link

1.3.16 du 25 juin 2021
----------------------
- `debug` debug rendre-link

1.3.15 du 19 juin 2021
----------------------
- `fixed` correction post bacasable qui était actif

1.3.14 du 15 juin 2021
----------------------
- `fixed` lien aide sur beedream dans README 

1.3.13 du 6 mai 2021
----------------------
- `fixed` ajout render-image pour prendre nen compte baseurl
- `changed` lien icones https://1.semantic-ui.com/elements/icon.html#/icons 

1.3.12 du 6 mai 2021
----------------------
- `fixed` carte sommaire non gérée par masonry dans index.html - ajout include grid.js

1.3.11 du 6 mai 2021
----------------------
- `fixed` carte sommaire non gérée par masonry dans index.html
- `changed` shortcode icone avec 4 arguments

1.3.10 du 4 mai 2021
----------------------
- `added` diaporama sur carte avec image et sans url
- `removed` render image

1.3.9 du 28 avril 2021
----------------------
- `added` viewer pdf texte
- `changed` beedream.css

1.3.8 du 27 avril 2021
----------------------
- `changed` shortcode repertoire download document

1.3.7 du 27 avril 2021
----------------------
- `changed` shortcode repertoire abandon utilisation de Page.Resource

1.3.6 du 27 avril 2021
----------------------
- `changed` shortcode repertoire check type word
- `changed` shortcode apropos - suppression du lien en bas de sommaire

1.3.5 du 27 avril 2021
----------------------
- `added` shortcode about
- `changed` icone about dans le footer du sommaire
- `removed` shortcode diapo

1.3.4 du 26 avril 2021
----------------------
- `removed` suppression spécificité env hugo

1.3.3 du 25 avril 2021
----------------------
- `fixed` url cover si baseurl

1.3.2 du 25 avril 2021
----------------------
- `fixed` shortcode carte open ds blank si http

1.3.1 du 25 avril 2021
----------------------
- `removed` shortcode galet
- `changed` shortcode repertoire qui utilise Page.resources

1.3 du 24 avril 2021
----------------------
- `fixed` correction chemin des cover dans les sommaires
- `changed` galerie avec vignette des images présentes dans le répertoire et sous-répertoires

1.2.3 du 23 avril 2021
----------------------
- `fixed` correction chemin des media et ressource pour prendre en compte une baseURL différente de "/"

1.2.2 du 20 avril 2021
----------------------
- `removed` template config
- `added` render-link render-image universels

1.2.1 du 18 avril 2021
----------------------
- `fixed` orthographe instaler/installer

1.2.0 du 13 avril 2021
----------------------
- `added` shortcode code

1.1.8 du 11 avril 2021
----------------------
- `fixed` diaporama qui ne fonctionnait pas dans page home

1.1.7 du 11 avril 2021
----------------------
- `fixed` relURL for icon and backgroundimage

1.1.6 du 11 avril 2021
----------------------
- `fixed` footer affichage

1.1.5 du 11 avril 2021
----------------------
- `fixed` footer article débordement si absence d'étiquettes

[1.1.4] - 2021.04.09
--------------------
- `fixed` liens symboliques relatifs

[1.1.3] - 2021.04.09
--------------------
- `changed` lien symbolique changelog.md readme.md config.yaml dans /site
- `changed` diaporama possible dans page d'accueil

[1.1.2] - 2021.04.08
--------------------
- `fixed` menu navigation qui n'était pas affiché en prod
- `changed` config.root.yaml

[1.1.1] - 2021.04.06
--------------------
- `changed` quickstart fond couleur
- `changed` cover par défaut

[1.1.0] - 2021.04.06
--------------------
- `changed` shortcode image avec pointer si dans diaporama
- `changed` font Google Jost par défaut
- `changed` documentation

[1.0.14] - 2021.04.03
--------------------
- `added` shortcode image possible dans diaporama
- `changed` font semantic par défaut
- `changed` documentation

[1.0.13] - 2021.03.25
--------------------
- `changed` enableSearch à false par défaut
- `changed` Label avec lien - dans nouvel onglet si préfixé par http
- `changed` toc - icône hashtag remplacé par chevron pour éviter confusion avec les liens tag
- `changed` documentation

[1.0.12] - 2021.03.23
--------------------
- `added` shortcode toc - table des matières des titres de niveau 2 seulement
- `added` shortcode label - label avec icone et lien

[1.0.11] - 2021.03.21
--------------------
- `changed` shortcode image - sans border margin et padding - `forme="ronde"`
- `changed` shortcode player - paramétre `boucle`
- `removed` shortcode radio - remplacé par `player` avec option `boucle`

[1.0.10] - 2021.03.18
--------------------
- `fixed` players non encadrés

[1.0.9] - 2021.03.18
--------------------
- `fixed` barre scroll verticale cachée désormais

[1.0.8] - 2021.03.18
--------------------
- `fixed` pointer sur player radio

[1.0.7] - 2021.03.15
--------------------
- `fixed` suppression scrollbar horizontal sur article

[1.0.6] - 2021.03.16
--------------------
- `fixed` suppression scrollbar sur card header

[1.0.5] - 2021.03.15
--------------------
- `fixed` débordement image plus grande que l'article

[1.0.4] - 2021.03.14
--------------------
- `fixed` affichage de l'image `cover` qui ne gérait pas le chemin lié à l'environnement

[1.0.3] - 2021.03.13
--------------------
- `changed` menu `main` renommer en `page`
- `changed` menu `card` renommer en `links`

[1.0.2] - 2021.03.12
--------------------
- fixed: chemin des images avec le préfixe de `baseURL` automatique car défini dans l'environnement `config/hugo/config.yaml`

[1.0.1] - 2021.03.11
--------------------
- fixed: Menu card - l'url doit se terminer par un /

[1.0.0] - 2021.03.11
--------------------
- added: Intégration du guide directement dans le thème `exampleSite`


###### Types de changements:
`added` *pour les nouvelles fonctionnalités.*  
`changed` *pour les changements aux fonctionnalités préexistantes.*  
`deprecated` *pour les fonctionnalités qui seront bientôt supprimées*.  
`removed` *pour les fonctionnalités désormais supprimées.*  
`fixed` *pour les corrections de bugs.*  
`security` *en cas de vulnérabilités.*  
