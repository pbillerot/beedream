---
title: Liste
draft: false 
date: 2021-02-20 
cover: /site/media/shortcode.svg
# Ne sera par affiché dans le sommaire
_build:
   list: false
menu: 
  main:
    parent: shortcode
---

```go-html-template
{{</* liste */>}} 
{{</* item icone="nom icone" texte="le texte..." lien="lien page ou site" */>}}
...
{{</* liste */>}} 
```
<!--more-->
> Pour présenter une liste avec des icônes  
La liste sera encadrée par la marque `liste`  
Les items devront préciser l'**icône** utilisée, le **texte** et éventuellement un **lien** vers une page

## Exemple
{{< liste >}} 
{{< item icone="marker" texte="Comité des Foires Porte Chalon 79400 Saint-Maixent l'École" lien="https://goo.gl/maps/Rb1W1BKu6sMeVV9P9" >}}
{{< item icone="mail" texte="contact@foire-expo-st-maixent.com" lien="mailto:contact@foire-expo-st-maixent.com" >}}
{{< item icone="phone" texte="05 49 05 76 25" >}}
{{< /liste >}} 

```go-html-template
{{</* liste */>}} 
{{</* item icone="marker" texte="Comité des Foires Porte Chalon 79400 Saint-Maixent l'École" lien="https://goo.gl/maps/Rb1W1BKu6sMeVV9P9" */>}}
{{</* item icone="mail" texte="contact@foire-expo-st-maixent.com" lien="mailto:contact@foire-expo-st-maixent.com" */>}}
{{</* item icone="phone" texte="05 49 05 76 25" >}}
{{</* /liste */>}} 
```
- <a href="https://fomantic-ui.com/elements/icon.html" target="_blank">Lien vers la bibliothèque d'icônes</a>
