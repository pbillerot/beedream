---
title: "Installer Beedream"
date: 2021-03-08
# expiryDate: 2021-03-11
draft: false
tags:
- technique
cover: "/site/media/installation.jpg"
style: bee-doc
menu:
  page:
    parent: site
    weight: 10 
---
<!--more-->
{{< toc >}}

## Installer Hugo

**[Hugo](https://gohugo.io)** est un moteur et générateur de site web statique à partir d'un fichier de configuration et de pages pour le contenu au format [Markdown](https://fr.wikipedia.org/wiki/Markdown).

L'installation est décrite sur le site [Hugo Quick Start](https://gohugo.io/getting-started/quick-start/)

Résumé des commandes

    # Sous DEBIAN 10
    # Installation de Hugo (actuellement version 0.77)
    sudo apt install hugo
    hugo version
    
    Hugo Static Site Generator v0.77.0-DEV linux/amd64 BuildDate: unknown

## Créer un site "quickstart"

    hugo new site quickstart

## Instaler le thème "beedream" avec Git

**Beedream** est un thème pour le moteur de site web statique [Hugo](https://gohugo.io)

Il sera considéré comme un sous-module du project **quickstart**

	# si cela n'est pas déjà fait, installer git
    sudo apt install git
    # 
    cd quickstart
    git init
    git submodule add https://github.com/pbillerot/beedream.git themes/beedream

## Déclarer le thème

    # - Déclaration du thème
    # - éditer le fichier "config.toml"
    # - ajouter la ligne "theme beedream"
    echo 'theme = "beedream"' >> config.toml

## Créer un premier document

    hugo new site/mon-premier-document.md
    # éditer le document pour changer l'état "draft:" à false

## Tester
Comme précisé dans la documentation de Hugo

	# lancer la commande
    hugo server

Démarrer votre navigateur avec l'adresse

- http://localhost:1313/

{{< image image="/site/media/quickstart.jpg" taille="l">}}
![](static/img/quickstart.jpg) 

## Mettre à jour le thème sur un site existant

    git submodule update --remote

## Installer le thème sur un site existant

    git submodule add https://github.com/pbillerot/beedream.git themes/beedream
    git submodule init
    git submodule update --remote

Changer `theme = "beedream"` dans `config.toml`

## Les répertoires d'un site Hugo

Lors de la création du site **quickstart** on retrouve l'organisation suivante : 
```
quickstart/
├── archetypes
│   └── default.md # le modèle des documents
├── config.toml    # fichier de configuration et de personnalisation du site
├── content        # le contenu du site
│   └── site
│       └── mon-premier-document.md
├── data           # données éventuelles
├── layouts        # modèles de présentation de certaines pages
├── resources      # fichiers de resource éventuelle
│   └── _gen
│       ├── assets
│       └── images
├── static         # fichiers css js image éventuels
└── themes         # répertoire des thèmes
    └── beedream
```
Avec **beedream**, pour simplifier on ne retiendra que les répertoires suivants :
```
quickstart/
├── config.toml    # fichier de configuration et de personnalisation du site
├── content        # le contenu du site
│   └── site
│       └── mon-premier-document.md
└── themes         # répertoire des thèmes
    └── beedream
```

