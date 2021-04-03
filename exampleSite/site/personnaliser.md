---
title: "Personnaliser le site"
date: 2021-03-08
draft: false
tags:
- contenu
cover: "/site/media/parametrage.jpg"
style: bee-doc
menu:
  page:
    parent: site
    weight: 20
---
<!--more-->
{{< toc >}}
## Le fichier de configuration d'un site Hugo
### config.toml
Le fichier `config.toml` placé à la racine du site utilise une sémantique [TOML](https://fr.wikipedia.org/wiki/TOML).
```toml
# config.toml
baseURL = "http://example.org/"
languageCode = "en-us"
title = "My New Hugo Site"

theme = "beedream"
```
### config.yaml
Personnelement je prèfère la sémantique [YAML](https://fr.wikipedia.org/wiki/YAML). Je vous propose de changer le fichier `config.toml` en `config.yaml` comme suit :
```yaml
# config.yaml
baseURL: "/"
languageCode: "fr-FR"
title: "My New Hugo Site"

theme: "beedream"
```
### markup
Les pages de contenu d'un site Hugo utilisent le langage [MARKDOWN](https://fr.wikipedia.org/wiki/Markdown) pour présenter et structurer le texte.  
Dès à présent nous allons ajouter des directives dans le fichier de config pour personnaliser le rendu propre à Beedream.

```yaml
# config.yaml
baseURL: "/"
languageCode: "fr-FR"
title: "My New Hugo Site"

theme: "beedream"
params:
  enableSearch: false
outputs:
  home: ["HTML", "RSS", "JSON"]
markup:
  goldmark:
    renderer:
      unsafe: true
  highlight:
    style: friendly # monokai dracula friendly
```

## Personnaliser le site
{{< image image="/site/captures/personnaliser-site.png" taille="m" position="droite" >}}
Beedream propose un site avec par défaut : un titre, sous-titre, avatar, favicon et fond d'écran.

Je vous propose de changer tous cela.

Pour se faire, nous allons ajouter des paramètres dans le paragraphe `params` du fichier config.
```yaml
# config.yaml
baseURL: "/"
languageCode: "fr-FR"
title: "My New Hugo Site"

theme: "beedream"
params:
  enableSearch: false

  # Personnalisation du site
  title: "TITRE DU SITE"
  subtitle: "Sous-titre du site"
  # l'image arrondie
  avatar: "/img/bee.svg"
  # l'icône dans l'onglet du navigateur
  favicon: "/img/hugoSM.png"
  # l'image d'arrière
  backgroundImage: "/img/beedream.jpg"

outputs:
  home: ["HTML", "RSS", "JSON"]
markup:
  goldmark:
    renderer:
      unsafe: true
  highlight:
    style: friendly # monokai dracula friendly
```
Les images utilisées ici sont celles de beedream sous `/themes/beedream/static/img`  
Nous allons recopier des images sous /content/site

    cp /themes/beedream/static/img/bg-bee.svg /content/site/bg-bee.svg
    cp /themes/beedream/static/img/icone-bee.svg /content/site/icone-bee.svg

et modifier `params` comme suit :
{{< image image="/site/captures/quickstart.png" taille="m" position="droite" >}}
```yaml

  # Personnalisation du site
  title: "Quick Start"
  subtitle: "Vroom..."
  # l'image qui sera arrondie à l'affichage 96x96px
  avatar: "/site/icone-bee.svg"
  # l'icône dans l'onglet du navigateur 96x96 px
  favicon: "/site/icone-bee.svg"
  # l'image d'arrière plan taille 900x1200 px
  backgroundImage: "/site/bg-bee.svg"

```

## Exemple de site
Le meilleur exemple est la documentation que vous êtes en train de lire.

Vous pouvez le recopier :

    cp /themes/beedream/exampleSite /content

{{< image image="/site/captures/exemple-site.png" taille="l" >}}

