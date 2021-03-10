---
title: "Readme"
date: 2021-03-07T09:26:06+01:00
draft: false
tags:
- news
- technique
# Ne sera par affiché dans le sommaire
_build:
   list: false

cover: "/site/media/readme.png"
---

THEME HUGO - BEEDREAM

<!--more-->

## Installation
L'installation est décrite sur le site [gohugo.io](https://gohugo.io)
- https://gohugo.io/getting-started/quick-start/

Résumé des commandes

    # Sous DEBIAN 10
    # Installation de Hugo
    sudo apt install hugo

# Création du site "quickstart"

    hugo new site quickstart

# Installation du thème "beedream"
    cd quickstart
    git init
    git submodule add https://github.com/pbillerot/beedream.git themes/beedream
    # - Déclaration du thème
    # - éditer le fichier "config.toml"
    # - ajouter la ligne "theme beedream"
    echo 'theme = "beedream"' >> config.toml

## Créer un premier document

    hugo new site/mon-premier-document.md
    # éditer le document pour changer l'état "draft:" à false

## Démarrage et Tests
Comme précisé dans la documentation de Hugo

    hugo server

Démarrer votre navigateur avec l'adresse

- http://localhost:1313/

![](static/img/quickstart.png)

## Mise à jour du thème sur un site existant

    git submodule update --remote

## Installation du thème sur un site existant

    git submodule add https://github.com/pbillerot/beedream.git themes/beedream
    git submodule init
    git submodule update --remote

Changer `theme = "beedream"` dans `config.toml`


