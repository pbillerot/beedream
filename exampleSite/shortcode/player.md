---
title: Player
draft: false 
date: 2021-02-20 
cover: /site/media/shortcode.svg
style: bee-doc
tags:
- shortcode
# Ne sera par affiché dans le sommaire
_build:
   list: false
menu: 
  page:
    parent: shortcode
---

```go-html-template
{{</* player "lien_vers_audio" ["titre"] ["boucle"] */>}}
```
<!--more-->
> player: Lecture du morceau de musique **en boucle** si le mot `boucle` est présent  
> Le lien peut être un flux radio en streaming  
> {{< texte rouge >}} {{< icone exclamation triangle >}} Si le mode `boucle` est utilisé le lien devra adresser un fichier local au serveur (*le lien n'est pas préfixé par `http://`*){{< /texte >}}

## Exemple
{{< player "/site/media/The Cure - The Boy Don't Cry - rythmes.wav" "boucle" "The Boy Don't Cry" >}}
{{< player "/site/media/Neil Young - Heart Of Gold.mp3" >}}
{{< player "https://jazzblues.ice.infomaniak.ch/jazzblues-high.mp3" "Radio Jazz Blues" >}}
{{< player "https://icecast.radiofrance.fr/franceinter-midfi.mp3" "Radio France Inter" >}}

```tpl
{{</* player "/site/media/The Cure - The Boy Don't Cry - rythmes.wav"  "boucle" "The Boy Don't Cry" */>}}
{{</* player "/site/media/Neil Young - Heart Of Gold.mp3" */>}}
{{</* player "https://jazzblues.ice.infomaniak.ch/jazzblues-high.mp3" "Radio Jazz Blues" */>}}
{{</* player "https://icecast.radiofrance.fr/franceinter-midfi.mp3" "France Inter" */>}}
```
> À noter que le titre par défaut affiché sera le nom du morceau sans l'extension.