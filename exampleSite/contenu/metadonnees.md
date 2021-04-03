---
title: "Les Métadonnées"
date: 2021-03-08
draft: false
tags:
- contenu
- metadonnees

cover: "/site/media/metadata.jpg"
style: bee-doc
menu:
  page:
    parent: contenu
    weight: 20
---
<!--more-->
L'entête de la page encadrée par des `---` sera constituée de **métadonnées** pour décrire la page et caractériser son contenu afin de faciliter son accès dans le site.

{{< toc >}}

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

# image de couverture dans le sommaire de la page
cover: /site/media/documents-illustration.jpg

# Ne sera pas affiché dans les listes de page
_build:
   list: false

# Style particulier de la page : bee-doc bee-chanson
style: bee-doc

# étiquettes pour classer la page et ainsi la retrouver sur le site
tags: 
- contenu

# catégories pour mettre la page dans un emplacement particulier
categories: 
- news 	# le lien de la page sera placé dans les actualités du Sommaire général

# Accrochage de la page dans le sommaire 
menu:
  # Dans le menu page
  page:
    weight: 10
    parent: shortcode

---

(résumé qui sera visible dans le sommaire de la page)

<!--more-->

(**contenu** de la *page*)

```
## Données de présentation
{{< cartes >}}

{{< carte titre="title" >}}
Le **titre** de la page
{{< /carte >}}

{{< carte titre="cover:" >}}
```yaml
cover: "/site/media/metadata.jpg"
```
L'image qui sera affichée dans le sommaire de la page lorsque celle-ci sera présentée dans une liste
{{< /carte >}}

{{< carte titre="style:" >}}{{< /carte >}}

{{< carte titre="_build:" >}}Associée avec le paramètre  
`list: false`  
pour cacher la page dans les listes {{< /carte >}}

{{< /cartes >}}

## Données de publication
{{< cartes >}}

{{< carte titre="draft:" >}}(**true** par défaut) la page **ne sera pas visible** sur le site{{< /carte >}}

{{< carte titre="date:" >}}La **date de création ou de modification**.  
Elle sera affichée en dessous du titre de la page si la date de publication n'est pas renseignée.{{< /carte >}}

{{< carte titre="publishDate:" >}}La **date de publication** de la page.  
La page ne sera visible qu'à **partir de cette date**.  
Elle sera affichée en dessous du titre de la page.{{< /carte >}}

{{< carte titre="expiryDate:" >}}La **date d'expiration** de la page.  
La page ne **sera plus visible** à partir de cette date.{{< /carte >}}

{{< /cartes >}}

## Données de catégorisation et de classement dans les menus
{{< cartes >}}

{{< carte titre="tags:" >}}{{< /carte >}}

{{< carte titre="categories:" >}}{{< /carte >}}

{{< carte titre="menu: page" >}}{{< /carte >}}

{{< /cartes >}}
