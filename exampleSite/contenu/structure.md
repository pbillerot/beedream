---
title: "Structure d'une page"
date: 2021-03-08
draft: false
tags:
- contenu
cover: "/site/media/gestion-documentation.jpg"
style: bee-doc
menu:
  page:
    parent: contenu
    weight: 10
---
<!--more-->
{{< toc >}}

Utilisons l'exemple de page  [/contenu/exemple-page/](../exemple-page/)

{{< image image="/site/captures/exemple-page.png" >}}

## Métadonnées

L'entête de la page encadrée par des `---` sera constituée de **métadonnées** pour décrire la page et caractériser son contenu afin de faciliter son accès dans le site.

```yaml
---
title: Exemple page
# Brouillon true ou false pour mettre la page en brouillon (elle ne sera pas visible sur le site)
draft: false 
# date de création
date: 2020-12-26 
# date de publication (la page sera visible à partir de cette date)
publishDate: 2021-02-10 
# date d'expiration (la page ne sera plus visible à partir de cette date)
expiryDate: 2021-05-01  

# étiquettes pour classer la page et ainsi la retrouver sur le site
tags: 
- contenu

# catégories pour mettre la page dans un emplacement particulier
categories: 
#- news 	# le lien de la page sera placé dans les actualités du Sommaire général

# image de couverture dans le sommaire de la page
cover: /site/media/documents-illustration.jpg

# Ne sera pas affiché dans les listes de page
_build:
   list: false

# Style particulier de la page : bee-doc bee-chanson
style: bee-doc

---

(résumé qui sera visible dans le sommaire de la page)

<!--more-->

{{</* image image="/site/media/contenu.jpg" taille="m" position="droite" */>}}

(**contenu** de la *page*)

```
Une [page spéciale](/contenu/metadonnees/) détaille toutes les métadonnées utilisables.

## Résumé
{{< image image="/site/captures/summary-example.png" taille="m" position="droite" >}}
Le texte placé entre `---` et `<!--more-->` sera présenté dans le sommaire de page dans les listes.

## Contenu

Le texte placé qui suit  `<!--more-->` est le contenu proprement dit de la page. 

La présentation du texte, gras souligné, les titres, les listes, les paragraphes seront indiqués par des balises dans le texte.
La syntaxe utilisée est le [markdown](/contenu/markdown/).

