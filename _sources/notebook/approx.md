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

# Approximation de l'optique géométrique

## Source lumineuse

````{important} __Source lumineuse__
:class: full-width

Une __source lumineuse__ est un objet qui émet de la lumière.

* On distingue les sources lumineuses _primaires_ qui produisent leurs propres lumières et les sources lumineuses _secondaires_ qui réémettent la lumière (ou une partie de la lumière) qu'ils reçoivent.
* Une __source lumineuse ponctuelle__ est une source lumineuse assimilable à un point. Il s'agit d'un modèle théorique mais qu'on peut considérer acceptable pour des sources lointaines (étoiles) ou pour des sources rendues très petites par un diaphragme [^diaphragme] très fin.
[^diaphragme]: Un diaphragme est un dispositif mécanique qui limitent l'étendue d'un faisceau lumineux. On peut le caractériser par sa forme et sa taille.
    * Une _source étendue_ est constituée d'un ensemble de sources ponctuelles. La majorité des sources que nous utilisons sont des sources étendues (lampes, soleil, lune, source secondaire sur terre... ).
* Une __source monochromatique__ est une source qui n'émet qu'une seule longueur d'onde.
````

````{sidebar} Exemples de sources
* Sources primaires: lampes, étoile, feu... 
* Sources secondaires: être humain, livre, Lune, planètes... 
````

## Faisceau lumineux et rayon lumineux

````{important} __Définition : Rayon lumineux__

Un __rayon lumineux__ est défini comme la direction de propagation de l'onde électromagnétique.
````

````{important} __Fondamental : Propagation de la lumière en milieu homogène (Admis)__

Dans un milieu homogène, transparent, et isotrope (MHTI), les ondes électromagnétiques __se propagent en ligne droite__. Les rayons lumineux sont donc des droites.
````


```{dropdown} MHTI
On définit les termes suivants:
* Homogène: les caractéristiques du milieu (comme son indice de réfraction) sont identiques en tout point du milieu
* Transparent: le milieu laisse passer la lumière ou au moins la partie du spectre étudié (spectre visible pour nous).
* Isotrope: Les caractéristiques du milieu sont les mêmes dans les différentes directions de l'espace (par exemple la vitesse de la lumière est la même dans toutes les directions de l'espace).
```

````{important} __Définition : Faisceau lumineux__

Un __faisceau lumineux__ est l'étendue de lumière issue d'un objet et - en général - passant par un diaphragme.

Un faisceau lumineux est composé d'un ensemble de rayons lumineux.

Outre le spectre de la lumière émise, un faisceau lumineux est caractérisé par son extension (sa forme et sa taille).

```{figure} ./images/faisceau-de-lumiere.png
:name: faisceau
:align: center
:width: 75%
Faisceau lumineux
```
````

## Rayon lumineux et diffraction

On peut voir un rayon lumineux comme un faisceau de  section ponctuelle (donc nulle). Une idée pour isoler un rayon lumineux est donc d'utiliser un diaphragme de section ponctuelle (donc nulle).

Celà permet d'avoir une vision de l'esprit de ce qu'est un rayon. En pratique, on peut chercher à le diaphragmer avec une section très très faible, mais... 


````{important} __Fondamental : Phénomène de diffraction__

Lorsqu'on essaie d'isoler un rayon lumineux comme précédemment et qu'on atteint une taille de diaphragme de l'ordre du micromètre (pour le visible - c'est-à-dire qu'elle devient de __l'ordre de la longueur d'onde__), la tâche augmente et l'on voit apparaître des anneaux autour de la tâche.

On parle de phénomène de __diffraction.__

Le phénomène de diffraction empêche de tendre rigoureusement vers un rayon lumineux isolé. Dans ces conditions, on ne peut même plus parler de rayon lumineux (il n'y a par exemple pas de correspondance entre un rayon avant et après le diaphragme.

```{figure} ./images/bog-isolons_un_rayon.png
:name: isolons
:align: center
Isoler un rayon lumineux
```
````

## Approximation de l'optique géométrique

````{important} __Définition : Cadre de l'optique géométrique__

On considère qu'on se place dans le cadre d'étude de __l'optique géométrique__ si l'on peut traiter un faisceau lumineux comme un ensemble de rayons lumineux.

Dans ce cadre, les rayons lumineux dans un milieu homogène, transparent et isotrope sont des lignes droites.
````

````{important} __Fondamental : Approximation de l'optique géométrique (Admis)__

On peut se placer dans le cadre de l'optique géométrique si les phénomènes de diffraction sont négligeable c'est-à-dire si __les caractéristiques du milieu (indice de réfraction) varient sur des distances grandes devant la longueur d'onde du milieu__ (ou ne varient pas).

````

````{dropdown} Distances caratéristiques de variation
Les "distances" de variations sont principalement pour nous la taille des diaphragmes et obstacles à la lumière que nous utilisons. Mais on peut étendre cette étude au cas où l'indice de réfraction varie continuement dans l'espace mais très "lentement " (dans l'espace, pas dans le temps). On peut penser à l'atmosphère dont l'indice de réfraction varie en fonction de l'altitude (ce qui cause les mirages par exemple).

Dans ce genre de systèmes, on peut alors s'intéresser à une distance "caractéristique" sur laquelle les variations d'indice de réfraction sont sensibles. C'est cette distance qui doit être comparée à la longueur d'onde. Ce cas d'étude sera très rarement abordés en première (ou en tout cas, nous admettrons que le cadre de l'optique géométrique est alors valable).
````

## Propriétés dans le cadre de l'optique géométrique

````{important} __Fondamental : Propagation rectiligne en MTHI__

On rappelle que dans un milieu homogène transparent et isotrope, les rayons lumineux se propagent en ligne droite.
````

````{important} __Fondamental : Indépendance des rayons__

Les rayons lumineux sont indépendants, c'est-à-dire que la propagation de l'un n'influe pas sur la propagation l'autre, même quand ils se croisent.
````

````{important} __Fondamental : Principe de retour inverse__

Si pour aller d'un point A à un point B, la lumière emprunte un chemin S. Alors pour aller du point B au point A, elle empruntera le chemin S en sens inverse.
````
