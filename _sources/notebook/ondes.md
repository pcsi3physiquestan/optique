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

````{important} __Définition : Indice de réfraction__
On définit l'indice de réfraction n d'un milieu par : $n = \frac{c}{c_{milieu}}$.

n est toujours supérieur ou égale à 1 et $c = 3 \times 10^8 m.s^{-1}$ est la vitesse de lalumière dans le vide.
````
````{sidebar} Célérité et milieu
Dans le vide, la célérité des ondes lumineuses est $c = 3 \times 10^8 m.s^{-1}$. Dans un autre milieu, la célérité de l'onde $c_{milieu}$ sera donc toujours inférieure à c.
````

````{admonition} Exemple - Indices de réfraction : valeurs
:class: note, dropdown

* L'indice de l'air est à peu près égal à 1. Il peut varier légèrement suivant la température et la densité (c'est la cause de mirage) et sa composition (propriété utilisée dans certains détecteurs de monoxyde de carbone).
* L'indice de l'eau liquide est d'environ 1,3 à température ambiante. Il a tendance à diminuer avec la température (mais la valeur donnée reste correcte entre 0$\circ$C et 100$\circ$C).
* L'indice du verre varie fortement en fonction de la nature du matériau. Il varie entre 1,4 et 1,7 (on peut monter à 1,8 pour certains verres ophtalmiques). En général, on prend comme moyenne 1,5 quand on n'a pas d'information.
* Les liquides ont aussi des indices de réfraction qui varie en fonction de leur nature et parfois en fonction de la concentration de certaines espèces. L'analyse de l'indice de réfraction d'un liquide - la réfractométrie - est une méthode d'analyse en chimie.
````

````{important} __Définition : Milieu dispersif__
Un milieu est dit __dispersif__ si son indice de réfraction dépend de la longueur d'onde.
````

````{admonition} Exemple - Exemple de milieux dispersifs.
:class: note, dropdown
C'est le cas de nombreux verre (utilisé dans les prismes) mais aussi de l'eau (principe de l'arc-en-ciel) - son indice de réfraction varie de 1,37 à 1,31 entre 200 et 1000nm.
````

## Relation entre célérité et longueur d'onde

````{important} __Fondamental : Relation fréquence-longueur d'onde__
On rappelle (Terminale) que pour une onde monochromatique de fréquence $\nu$, de longueur d'onde $\lambda$ et de célérité $c_0$, on la relation :

\begin{equation}
\lambda \nu = c_0
\end{equation}
````

````{dropdown} La fréquence ne varie pas
Pour un signal monochromatique donné, la fréquence ne varie pas lorsque le signal passe d'un milieu à un autre.

Conséquence : Puisque la célérité varie, la longueur d'onde aussi. Si le signal possède une longueur d'onde $\lambda_0$ dans le vide, dans un milieu d'indice de réfraction n, la célérité est ainsi $\frac{c}{n}$ et la longueur d'onde est donc $\lambda = \frac{\lambda_0}{n}$.

Lorsqu'on veut étudier la propriété d'un signal lumineux (type de rayonnement, couleur), les données référencées concernant __la longueur d'onde dans le vide__.

Exemple : les longueurs d'onde du visible données $400nm ;800nm$ sont des longueurs d'onde dans le vide.
````

