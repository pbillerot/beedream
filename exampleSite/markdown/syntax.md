---
title: Syntaxe Markdown
draft: false 
date: 2021-02-23
tags:
- markdown
cover: /markdown/markdown.jpg
#cover: /markdown/markdown-embed.png
menu:
  main:
    weight: 2
---
Toutes les balises du Markdown pour présenter le contenu dans les pages.
<!--more-->

> **Markdown** est un langage de balisage léger dans le but d'offrir une syntaxe facile à lire et à écrire. Un document balisé par Markdown sera converti en HTML pour être affiché dans le site web.
À l'image des outils de traitement de texte comme Word, Markdown va nous permettre de gérer le contenu et la présentation du texte dans la page.

Ci-après les différentes balises du Markdown pour présenter le texte

## Titre
{{< colonnes two >}}
```tpl
# Titre 1
## Titre 2
### Titre 3
#### Titre 4
##### Titre 5
###### Titre 6

Une alternative pour Titre1 et Titre2, on peut souligner :

Alternative-Titre1
==================

Alternative-Titre2
------------------
```
<--->

# Titre 1
## Titre 2
### Titre 3
#### Titre 4
##### Titre 5
###### Titre 6

Une alternative pour Titre1 et Titre2, on peut souligner :

Alternative-Titre1
==================

Alternative-Titre2
------------------

{{< /colonnes >}}

## Accentuation
{{< colonnes two >}}

```tpl
Italique, avec des *astérisques* ou des _traits de soulignement_.

Gras, avec des doubles **astérisques** ou des doubles __traits de soulignement__ .

Combinaison avec des **astérisques et des traits de _soulignement_** .

Barré avec deux tildes. ~~Grattez ça~~ .
```

<--->

Italique, avec des *astérisques* ou des _traits de soulignement_ .

Gras, avec des doubles **astérisques** ou des doubles __traits de soulignement__ .

Combinaison avec des **astérisques et des traits de _soulignement_** .

Barré avec deux tildes. ~~Grattez ça~~.

{{< /colonnes >}}

## Listes
{{< colonnes two >}}
```tpl
1. Premier élément de liste ordonné
2. Un autre article
   * Sous-liste non ordonnée.
1. Les chiffres réels n'ont pas d'importance, juste que c'est un nombre
   1. Sous-liste ordonnée
   1. Sous-liste ordonnée suite
4. Et un autre article.

   Vous pouvez avoir des paragraphes correctement indentés dans les éléments de liste. Remarquez la ligne vide ci-dessus et les espaces de début (au moins un, mais nous en utiliserons trois ici pour aligner également le Markdown brut).

   Pour avoir un saut de ligne sans paragraphe, vous devrez utiliser deux espaces de fin.
   Notez que cette ligne est séparée, mais dans le même paragraphe...  

* Une liste non ordonnée peut utiliser des astérisques
- Ou moins
+ Ou plus
```
<--->
1. Premier élément de liste ordonné
2. Un autre article
   * Sous-liste non ordonnée.
1. Les chiffres réels n'ont pas d'importance, juste que c'est un nombre
   1. Sous-liste ordonnée
   2. Sous-liste ordonnée suite
4. Et un autre article.

   Vous pouvez avoir des paragraphes correctement indentés dans les éléments de liste. Remarquez la ligne vide ci-dessus et les espaces de début (au moins un, mais nous en utiliserons trois ici pour aligner également le Markdown brut).
   
   Pour avoir un saut de ligne sans paragraphe, vous devrez utiliser deux espaces de fin.
   Notez que cette ligne est séparée, mais dans le même paragraphe.  

* Une liste non ordonnée peut utiliser des astérisques
- Ou moins
+ Ou plus
{{< /colonnes >}}

## Liens
{{< colonnes two >}}
```tpl
[Je suis un lien](https://www.google.com)

[Je suis un lien avec un titre](https://www.google.com "Google's Homepage")

[je suis un lien vers une référence][Texte de Référence]

[On peut utiliser un N° pour une référence ][1]

Ou laissez-le vide et utilisez le [texte du lien lui-même]

Les URL et les URL entre crochets seront automatiquement transformées en liens. http://www.example.com ou <http://www.example.com>.

Du texte pour montrer que les liens de référence ne seront pas affichés.

[Texte de Référence]: https://www.mozilla.org
[1]: http://slashdot.org
[texte du lien lui-même]: http://www.reddit.com
```
<--->

[Je suis un lien](https://www.google.com)

[Je suis un lien avec un titre](https://www.google.com "Google's Homepage")

[je suis un lien vers une référence][Texte de Référence]

[On peut utiliser un N° pour une référence ][1]

Ou laissez-le vide et utilisez le [texte du lien lui-même]

Les URL et les URL entre crochets seront automatiquement transformées en liens. http://www.example.com ou <http://www.example.com>.

Du texte pour montrer que les liens de référence ne seront pas affichés.

[Texte de Référence]: https://www.mozilla.org
[1]: http://slashdot.org
[texte du lien lui-même]: http://www.reddit.com
{{< /colonnes >}}

## Images
{{< colonnes two >}}
```tpl
Voici notre logo (survolez pour voir le texte du titre):

Style en ligne: ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Titre Texte 1")

Style de référence: 
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Titre Texte 2"
```
<--->
Voici notre logo (survolez pour voir le texte du titre):

Style en ligne: ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Titre Texte 1")

Style de référence: 
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Titre Texte 2"
{{< /colonnes >}}

## Tables
{{< colonnes two >}}
```tpl
Les 2 points sont utilisés pour alignre les colonnes.
| Tables         | Sont            | Frais  |
| -------------- |:---------------:| ------:|
| col 3 est      | aligné à droite | 1600 € |
| col 2 est      | centré          |   12 € |
| lignes zébrées | harmonieuses    |    1 € |

Il doit y avoir au moins 3 tirets séparant chaque cellule d'en-tête. Les barres externes (|) sont facultatives, et vous n'avez pas besoin d'aligner les barres. Vous pouvez également utiliser du code Markdown en ligne.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
```
<--->
Les 2 points sont utilisés pour alignre les colonnes.

| Tables         | Sont            | Frais  |
| -------------- |:---------------:| ------:|
| col 3 est      | aligné à droite | 1600 € |
| col 2 est      | centré          |   12 € |
| lignes zébrées | harmonieuses    |    1 € |

Il doit y avoir au moins 3 tirets séparant chaque cellule d'en-tête. Les barres externes (|) sont facultatives, et vous n'avez pas besoin d'aligner les barres. Vous pouvez également utiliser du code Markdown en ligne.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
{{< /colonnes >}}

## Bloc de citation
{{< colonnes two >}}
```tpl
>Les bloc de citation sont très pratiques dans les e-mails pour émuler le texte de réponse.
>Cette ligne fait partie du même bloc.

Saut de citation.

> Il s'agit d'une très longue ligne qui sera toujours citée correctement lorsqu'elle se terminera. Oh mon garçon, continuons à écrire pour nous assurer que cela est assez long pour que tout le monde puisse en profiter. Oh, vous pouvez mettre de code **Markdown** dans un bloc de citation.
```
<--->
>Les bloc de citation sont très pratiques dans les e-mails pour émuler le texte de réponse. Cette ligne fait partie du même devis.

Saut de citation.

> Il s'agit d'une très longue ligne qui sera toujours citée correctement lorsqu'elle se terminera. Oh mon garçon, continuons à écrire pour nous assurer que cela est assez long pour que tout le monde puisse en profiter. Oh, vous pouvez mettre du code **Markdown** dans un bloc de citation.
{{< /colonnes >}}

## HTML en ligne
{{< colonnes two >}}
Vous pouvez également utiliser du HTML brut dans votre Markdown, et cela fonctionnera plutôt bien.

```tpl
<dl>
  <dt>Liste de définitions</dt>
  <dd>Est-ce quelque chose que les gens utilisent parfois.</dd>
  <dt>Markdown in HTML</dt>
  <dd>Ne fonctionne *pas* **très** bien. Utilisez des <em>balises</em> HTML.</dd>
</dl>
```
<--->
<dl>
  <dt>Liste de définitions</dt>
  <dd>Est-ce quelque chose que les gens utilisent parfois.</dd>
  <dt>Markdown in HTML</dt>
  <dd>Ne fonctionne *pas* **très** bien. Utilisez des <em>balises</em> HTML.</dd>
</dl>
{{< /colonnes >}}

## Ligne horizontale
{{< colonnes two >}}
```tpl
Trois ou plus...
---
tirets
***
astérisques
___
soulignés
```
<--->
Trois ou plus...
---
tirets
***
astérisques
___
soulignés
{{< /colonnes >}}

## Sauts de ligne
Ma recommandation de base pour apprendre comment fonctionnent les sauts de ligne est d'expérimenter et de découvrir - appuyez une fois sur <Entrée> (c'est-à-dire, insérez une nouvelle ligne), puis appuyez deux fois (c'est-à-dire, insérez deux nouvelles lignes), voyez ce qui se passe. Vous apprendrez bientôt à obtenir ce que vous voulez. "Markdown" est votre ami.
{{< colonnes two >}}
```tpl
Voici une ligne pour nous de commencer.

Cette ligne est séparée de celle ci-dessus par deux nouvelles lignes, ce sera donc un paragraphe séparé.

Cette ligne commence également un paragraphe séparé, mais ...bb
Cette ligne n'est séparée que par un seul saut de ligne, c'est donc une ligne distincte dans le même paragraphe .
```
<--->
Voici une ligne pour nous de commencer.

Cette ligne est séparée de celle ci-dessus par deux nouvelles lignes, ce sera donc un paragraphe séparé.

Cette ligne commence également un paragraphe séparé, mais ...  
Cette ligne n'est séparée que par un seul saut de ligne, c'est donc une ligne distincte dans le même paragraphe. _(deux espaces ont dû être ajoutés à la fin de la 1ère ligne)_
{{< /colonnes >}}