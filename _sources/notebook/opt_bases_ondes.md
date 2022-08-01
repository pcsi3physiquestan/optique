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
# La lumière est une onde 

````{margin}
On rappelle que les expériences réalisées en physique classique (principalement les phénomènes de diffraction et d'interférences) poussent à traiter la lumière comme une onde.
````

## Célérité et indice de réfraction

Une onde se propage à une vitesse - une célérité - donnée qui dépend du milieu dans lequel elle se déplace.

````{important} __Indice de réfraction et milieu dispersif.__
:class: full-width

On définit l'indice de réfraction n d'un milieu par : $n = \frac{c}{c_{milieu}}$.

* n est toujours supérieur ou égale à 1 et $c = 3 \times 10^8 m.s^{-1}$ est la vitesse de lalumière dans le vide.

* Un milieu est dit __dispersif__ si son indice de réfraction dépend de la longueur d'onde.
````
````{sidebar} Célérité et milieu
Dans le vide, la célérité des ondes lumineuses est $c = 3 \times 10^8 m.s^{-1}$. _Dans un autre milieu, la célérité de l'onde $c_{milieu}$ sera toujours inférieure à c_.
````


````{topic} Exemples
:class: full-width
| Milieu | Indice | Remarques |
|:-|:-:|:-|
| Air | $\approx 1$ | Varie très légèrement suivant sa température, sa densité (mirage) et sa composition (utilisé dans des détecteurs de monoxyde de carbone). Peu dispersif. |
| Eau liquide | $\approx 1,3$ | Entre $0 ^{\circ} C$ et $100 ^{\circ} C$. Diminue avec la température. Dispersif (arc-en-ciel). |
| Verre | (1,5) 1,4 -- 1,7 | Varie fortement suivant le verre. Dispersif.|
| Liquide | | Variables suivant leur nature. Utile pour la réfractométrie en chimie. Dispersif.|
````

## Relation entre célérité et longueur d'onde

````{important} __Relation fréquence-longueur d'onde__
:class: full-width
On rappelle que pour une onde monochromatique de fréquence $\nu$, de longueur d'onde $\lambda$ et de célérité $c_0$, on la relation :

$$
\lambda \nu = c_0
$$
````


