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
- news 	# le lien de la page sera placé dans les actualités du Sommaire général

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
## Métadonnées

L'entête de la page encadrée par des `---` sera constituée de **métadonnées** pour décrire la page et caractériser son contenu afin de faciliter son accès dans le site.
{{< cartes taille="m" >}}

{{< carte titre="title:" >}}Le **titre** de la page{{< /carte >}}

{{< carte titre="draft:" >}}(**true** par défaut) la page **ne sera pas visible** sur le site{{< /carte >}}

{{< carte titre="date:" >}}La **date de création ou de modification**.  
Elle sera affichée en dessous du titre de la page si la date de publication n'est pas renseignée.{{< /carte >}}

{{< carte titre="publishDate:" >}}La **date de publication** de la page.  
La page ne sera visible qu'à **partir de cette date**.  
Elle sera affichée en dessous du titre de la page.{{< /carte >}}

{{< carte titre="expiryDate:" >}}La **date d'expiration** de la page.  
La page ne **sera plus visible** à partir de cette date.{{< /carte >}}

{{< carte titre="tags:" >}}{{< /carte >}}

{{< carte titre="categories:" >}}{{< /carte >}}

{{< carte titre="cover:" >}}{{< /carte >}}

{{< carte titre="menu:" >}}{{< /carte >}}

{{< carte titre="style:" >}}{{< /carte >}}

{{< carte titre="_build:" >}}Associée avec le paramètre  
`list: false`  
pour cacher la page dans les listes {{< /carte >}}

{{< /cartes >}}

## Résumé

## Contenu
Une page d'un site Hugo est un fichier texte avec la syntaxe **Markdown** décrite [dans cette page](/contenu/markdown/).


