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
# Instruments d'optique

````{admonition} Compétences
* Modéliser à l'aide de plusieurs lentilles un dispositif optique d'utilisation courante.
* Connaître les positions relatives des éléments d'un système afocal à deux lentilles.
* Savoir calculer des éléments caractéristiques (grossissement, grossissement commercial, profondeur de champ) pour un instrument d'optique donné (leur définition étant donnée).
````

````{admonition} Intérêt d'un instrument d'optique
:class: hint, dropdown
Un instrument d'optique peut avoir plusieurs buts suivant les raisons de son utilisation. On distingue les instruments d'optique devant être utilisés par l'oeil (loupe, lunette... ) et les instruments d'optique servant à projeter l'image (en vue d'un enregistrement: l'appareil photographique).

Nous allons surtout développer l'étude des premiers (une activité sera proposée sur l'appareil photographique). Ces instruments ont en général pour but de permettre l'observation d'objets dans les meilleures conditions c'est-à-dire:

* l'image (finale) donnée par l'instrument sera placée au Punctum Remotum de l'oeil de l'utilisateur. Cette image sert d'bojet pour l'oeil.
* l'image (finale) est en générale "grossie", c'est-à-dire que __l'angle sous laquelle on la voit avec l'instrument sera plus grand que l'angle sous lequel on la voyait à l'oeil nu.__
````

````{admonition} Cas d'étude canonique
:class: hint, dropdown
L'étude canonique consiste à analyser les caractéristiques d'un instrument dans le cadre d'une utilisation par un __oeil emmétrope.__

Conséquence: On cherchera à placer l'image finale __à l'infini.__. On étudiera très souvent les caractéristiques de l'instrument dans ce cadre.
````

````{dropdown} Cas de l'utilisation par un oeil myope
En général, les instruments sont analysés par le constructeur dans le cadre canonique précédent (on parle de caractéristiques "commerciales"). Mais une bonne partie des instruments proposent un réglage (l'oculaire - cf. suite) permettant d'adapter l'appareil à un utilisateur myope.
````

````{important} __Définition : Système afocal__
Un système __afocal__ est un système donnant d'un objet à l'infini une image finale à l'infini.
````

````{admonition} Intérêt des systèmes afocaux
:class: hint, dropdown
Les systèmes afocaux sont très courants, notamment en astronomie car ils permettent de visualiser de manière grossie (dans le cadre canonique évoqué précédemment) des objets très lointains (étoiles, planètes... ).
````

````{important} __Définition : Autres systèmes.__
Il est bien évident qu'il existe d'autres systèmes visant des objets à distance finie: loupe, microscope, viseurs... 

Dans le cadre d'utilisation canonique, ces instruments renvoient néanmoins l'image finale à l'infini.
````

## Caractéristiques générales: Champ, résolution et profondeur de champ

````{admonition} Champ angulaire
:class: hint, dropdown
On rappelle que le champ angulaire est l'écart angulaire maximal pouvant être vue par l'instrument d'optique.

_En pratique, le champ angulaire dépend du système d'observation derrière l'instrument (en pratique l'oeil de l'observateur). C'est pourquoi on parle en général du champ angulaire du système {instrument + oeil}._
````


````{admonition} Pouvoir de résolution
:class: hint, dropdown
On rappelle que le pouvoir de résolution est l'angle minimal nécessaire pour pouvoir distinguer (résoudre) deux objets visés.
````

````{admonition} Profondeur de champ
:class: hint, dropdown
On rappelle que la profondeur de champ est l'intervalle de position permettant d'être vue nette à travers l'instrument pour un réglage donné.
````

````{admonition} Latitude de mise au point
:class: hint, dropdown
On définit la latitude de mise au point comme la gamme de réglage (et position) possible de l'instrument d'optique permettant à l'oeil de l'observateur d'observer l'objet net (l'image finale vue donnée par l'instrument - donc l'objet vu par l'oeil - doit être entre le Punctum Proximum et le Punctum Remotum). La latitude de mise au point dépendant de l'oeil de l'observateur, on déterminer implicitement la latitude de mise au point du système {instrument + oeil}
````

````{dropdown} Latitude et position de l'objet
Dans les calculs théoriques, la recherche de la latitude de mise au point correspond à rechercher les positions de l'objet donnant une image finale entre le PP et le PR (On bouge l'objet et non l'instrument).

Mais en pratique, la latitude de mise au point est plus souvent associée à la latitude donnée à un réglage (par exemple le réglage d'un objectif) pour observer l'objet net. Cette latitude de mise au point peut-être un avantage (réglage plus souple) ou un inconvénient (cf. TP).
````

## Le grossissement

Nous avons dans les chapitres précédents évoquer le grandissement et donc la taille des objets mais cette donnée seule a peu d'intérêt.

En effet, pour une image non ponctuelle à l'infini, sa taille est en générale...  infinie ! Mais il peut paraître plus petit (ou pas) vu qu'il est très loin !

Dans ces conditions, on utilisera plutôt le concept de grossissement basé sur les __angles__ apparent, c'est-à-dire l'angle sous lequel on voit l'objet (on traitera toujours des objets à 2D).

````{important} __Définition : Grossissement__

On définit le __grossissement__ d'un instrument d'optique comme le rapport (en valeur absolue) de l'angle sous lequel on voit l'objet à travers l'instrument d'optique sur l'angle sous lequel on voit l'objet à l'oeil nu.
````

````{dropdown} Cadre d'utilisation du grossissement
La limite du grossissement dans le cas général est qu'il dépend de la position de l'objet visé (si l'image n'est pas renvoyé à l'infini) et de la position de l'oeil (si l'objet n'est pas à l'infini).

C'est pourquoi, on utilisera le grossissement principalement __pour les instruments d'optique afocaux.__

Comme nous allons le voir, pour les instruments visant un objets à distance finie, les constructeurs donnent une donnée commercial dans une utilisation canonique: on calcule ou mesure le grossissement dans des conditions optimales: l'image finale sera à l'infini et l'angle à l'oeil nu est le plus grand possible, d'où la définition:
````

````{important} __Définition : Grossissement commercial__
On définit le __grossissement commercial__ d'un instrument d'optique comme le rapport (en valeur absolue) de l'angle sous lequel on voit l'objet à travers l'instrument d'optique __lorsque l'image finale est à l'infini__ sur l'angle sous lequel on voit l'objet à l'oeil nu __lorsque l'objet est placé au Punctum Proximum de l'oeil soit à d=25cm__ (soit l'angle maximal sous lequel on peut voir l'objet à l’oeil nu).
````

````{dropdown} Positions de l'objet
Dans le cadre de la mesure du grossissement commercial, l'objet ne sera probablement placé de la même manière lorsqu'on mesure l'angle à l'oeil nu et l'angle à travers l'instrument.
````
