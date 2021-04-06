---
title: "Les Vues"
date: 2021-04-01
draft: false
tags:
- contenu
cover: "/site/media/naviguer.jpg"
style: bee-doc
menu:
  page:
    parent: site
    weight: 30
---
Beedream propose 3 vues différentes du site
<!--more-->
{{< toc >}}
{{< diaporama >}}

## La vue Accueil
{{< image image="/site/captures/vue-accueil.png" taille="l" position="droite" >}}

Si un document `_index.md` est placé directement sous la racine du site, celui-ci sera affiché à la droite de la carte sommaire.  
Sinon c'est la vue Étiquette qui sera affichée.

## La vue Étiquette
{{< image image="/site/captures/vue-etiquette.png" taille="l" position="droite" >}}

La sélection d'une "étiquette" (_tag_) dans le sommaire va lister toutes les pages marquées avec cette étiquette.

{{< image image="/site/captures/summary.png" taille="s" >}}

```tpl
---
title: "Les Vues"
date: 2021-04-01
draft: false
tags:
- contenu
cover: "/site/media/naviguer.jpg"
style: bee-doc
menu:
  page:
    parent: site
    weight: 30
---
```
À noter que cette dans cette vue que la métadonnée `cover` de la page est utilisée.  
Si la métadonnée `cover` n'est pas renseignée une couverture aléatoire par défaut sera appliquée.

## La vue Article
{{< image image="/site/captures/vue-article.png" taille="l" position="droite" >}}

La vue "article" va afficher le contenu de l'article.
