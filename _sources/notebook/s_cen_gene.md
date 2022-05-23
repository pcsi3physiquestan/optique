---
jupytext:
  encoding: '# -*- coding: utf-8 -*-'
  formats: ipynb,md:myst
  split_at_heading: true
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.10.3
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---
# Systèmes centrées: présentation générales

## Systèmes centrées: définition

````{important} __Systèmes optiques centrés et caractéristiques__
:class: full-width
Un système centré est un système optique - c'est-à-dire une série de dioptre (et de surfaces réfléchissantes) - possédant un axe de révolution.

* L'axe de révolution d'un système optique centré est appelé __axe optique__.
* Tout plan perpendiculaire à l'axe optique est appelé __plan frontal.__
````


```{figure} ./images/optique_sys_centres.jpg
:name: systeme_centre
:align: center
```

## Rayons entrants et sortants

````{margin}
On parle aussi de rayon _réfléchi_ pour un rayon sortant d'un système optique après réflexion sur un miroir.
````

````{important} __Définition : Rayons entrants (ou incidents) et sortants ou transmis__
:class: full-width

* Les rayons qui arrivent sur le système optique sont appelés __rayons entrants ou rayons incidents__.
    * La portion réellement parcourue par le rayon est appelé __rayon réel__. Son prolongement est appelé __rayon virtuel__.

* Les rayons qui sortent du système optique sont appelés __rayons sortants ou rayons transmis__.
    * La portion réellement parcourue par le rayon est appelé __rayon réel__. Son prolongement est appelé __rayon virtuel__.
````

```{figure} ./images/optique_sys_centres_virtuel.jpeg
:name: virtuel
:align: center
```

## Objets réels et virtuels

````{important} __Définition : Objet ponctuel__
Lorsque les rayons entrants concourent en un point, on appelle ce point, __point objet (ou objet)__.

* Si le point objet est le concours des rayons réels, alors on dit que l'objet est réel (comme $A_1$ sur la figure ci-dessous).
* Si le point objet est le concours du prolongements des rayons réels (rayons virtuels), on dit que l'objet est virtuel (comme $A_2$). Un objet virtuel est nécessairement formé par un système optique en amont.

````

```{figure} ./images/optique_objet_virtuel_reel.jpg
:name: virtuel_reel
:align: center
```

````{topic} Repérage d'un objet
On repérera un point objet par:

```{figure} ./images/optique_objet_reperage.jpg
:name: reperage
:align: center
```

* sa _position longitudinale_, c'est-à-dire la position du plan frontal où se trouve le point objet sur l'axe optique (donc la position du point A sur le graphique). L'axe optique est orienté et les distance sont algébriques (notée $\overline{OA}$).
* sa _position transversale_, c'est-à-dire l'écart à l'axe optique. A nouveau, on travaille sur un axe orienté perpendiculaire à l'axe optique (on rappelle que la symétrie axiale permet de travailler sur un seul axe du plan frontal). Les positions sont donc algébriques  (notée $\overline{AB}$).

```{attention}
:class: dropdown
__Nature de l'objet__

Un objet n'est pas nécessairement matériel (source primaire ou secondaire), il peut être aussi formé au concours de rayons transmis par un premier système optique (on dira qu'il est l'image - cf. suite - donnée par le premier système optique) avant d'entrée dans le second système optique (dont il est donc l'objet).

Exemple: Un oeil humaine utilise un télescope. Le téléscope vise une étoile (qui est un objet pour le téléscope) et en donne une image (grossie normalement). C'est cette image qui est vue par l'oeil. Elle est donc l'objet pour système optique {oeil} (plus exactement le cristalin).
```
````
