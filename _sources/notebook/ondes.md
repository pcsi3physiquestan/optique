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


````{topic} __Exemples__
:class: full-width
| Milieu | Indice | Remarques |
|:-|:-:|:-|
| Air | $\approx 1$ | Varie très légèrement suivant sa température, sa densité (mirage) et sa composition (utilisé dans des détecteurs de monoxyde de carbone). Peu dispersif. |
| Eau liquide | $\approx 1,3$ | Entre $0 ^{\circ} C$ et $100 ^{\circ} C$. Diminue avec la température. Dispersif (arc-en-ciel). |
| Verre | (1,5) 1,4 -- 1,7 | Varie fortement suivant le verre. Dispersif.|
| Liquide | | Variables suivant leur nature. Utile pour la réfractométrie en chimie. Dispersif.|
````

## Relation entre célérité et longueur d'onde

<!-- ````{sidebar} La fréquence ne varie pas
Pour un signal monochromatique donné, la fréquence ne varie pas lorsque le signal passe d'un milieu à un autre.

* Conséquence : Puisque la célérité varie, la longueur d'onde aussi. Si le signal possède une longueur d'onde $\lambda_0$ dans le vide, dans un milieu d'indice de réfraction n, la célérité est ainsi $\frac{c}{n}$ et la longueur d'onde est donc $\lambda = \frac{\lambda_0}{n}$.
* Lorsqu'on veut étudier la propriété d'un signal lumineux (type de rayonnement, couleur), les données référencées concernant __la longueur d'onde dans le vide__.

Exemple : les longueurs d'onde du visible données $400nm ;800nm$ sont des longueurs d'onde dans le vide.
```` -->
````{important} __Relation fréquence-longueur d'onde__
:class: full-width
On rappelle (Terminale) que pour une onde monochromatique de fréquence $\nu$, de longueur d'onde $\lambda$ et de célérité $c_0$, on la relation :

\begin{equation}
\lambda \nu = c_0
\end{equation}
````


