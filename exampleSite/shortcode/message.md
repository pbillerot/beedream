---
title: Message
draft: false 
date: 2021-02-22 
cover: /site/media/shortcode.svg
tags:
- shortcode
# Ne sera par affiché dans le sommaire
_build:
   list: false
menu: 
  page:
    parent: shortcode
---
```tpl
{{</* message [info success warning error] */>}} message {{</* /message */>}}
```
<!--more-->

> Pour afficher un paragraphe d'informations, d'avertissements d'erreurs encadré et en couleur en fonction du type `info` `success` `warning` `error`

{{< message info >}}
 Texte du message de type **info**
{{< /message >}}

{{< message success >}}
Texte du message de type **success**
{{< /message >}}

{{< message warning >}}
Texte du message de type **warning**
{{< /message >}}

{{< message error >}}
Texte du message de type **error**
{{< /message >}}

{{< message >}}
Texte du message sans préciser le type
{{< /message >}}

## Exemple

{{< message warning >}}
### Tout membre peut se retirer d’une association

La **loi du 1er juillet 1901**, depuis son origine, prévoyait que seuls les membres d’une association formée pour une durée illimitée pouvaient se retirer après paiement des cotisations échues et de l’année courante.
{{< /message >}}

```tpl
{{</* message warning */>}}
### Tout membre peut se retirer d’une association

La **loi du 1er juillet 1901**, depuis son origine, prévoyait que seuls les membres d’une association formée pour une durée illimitée pouvaient se retirer après paiement des cotisations échues et de l’année courante.
{{</* /message */>}}
```
