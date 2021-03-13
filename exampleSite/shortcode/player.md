---
title: Player & Radio
draft: false 
date: 2021-02-20 
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

```go-html-template
{{</* player "lien_vers_audio" "titre" */>}}
{{</* radio "lien_vers_station" "titre" */>}}
```
<!--more-->
> player: Lecture du morceau de musique **en boucle**  
> radio: Lecture du flux radio en streaming  

## Exemple
{{< player "/site/media/The Cure - The Boy Don't Cry - rythmes.wav" "The Boy Don't Cry">}}
{{< radio "http://jazzblues.ice.infomaniak.ch/jazzblues-high.mp3" "Radio Jazz Blues" >}}
{{< radio "https://icecast.radiofrance.fr/franceinter-midfi.mp3" "Radio France Inter" >}}

```tpl
{{</* player "/site/media/The Cure - The Boy Don't Cry - rythmes.wav" "The Boy Don't Cry" */>}}
{{</* radio "http://jazzblues.ice.infomaniak.ch/jazzblues-high.mp3" "Radio Jazz Blues" */>}}
{{</* radio "https://icecast.radiofrance.fr/franceinter-midfi.mp3" "France Inter" */>}}
```
