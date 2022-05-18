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

# Lois de Snell-Descartes

Les lois de Snell-Descartes permettent de traiter le cas où l'on passe brusquement d'un milieu d'indice de réfraction $n_1$ à un milieu d'indice $n_2$.

````{margin}
On remarquera que localement, l'approximation de l'optique géométrique n'est plus valable. Cela explique que les propriétés précédentes ne suffisent plus à étudier le comportement des rayons lumineux.
````

## Lois de Snell-Descartes: Enoncé


````{topic} Définitions préalables
On considère un rayon lumineux, appelé __rayon incident__ qui se propage dans un milieu d'indice $n_1$ et qui arrive à la frontière - le __dioptre__ avec un milieu d'indice $n_2$ différent de $n_1$.

On définit la normale au dioptre (n) au point d'incidence I où le rayon incident intersecte le dioptre et on appelle __plan d'incidence__ le plan formé par le rayon incident et la normale (n) au dioptre.
````


````{important} __Lois de Snell-Descartes (Admis)__

Lorsqu'un rayon lumineux (appelé __rayon incident__) se propageant dans un milieu d'indice $n_1$ arrive sur un __dioptre__, ce rayon sépare énergétiquement en deux rayons __tous deux contenus dans le plan d'incidence__:

* l'un, appelé __rayon réfléchi__, continue à se propager dans le milieu d'indice $n_1$.
* l'autre, appelé __rayon réfracté__, se propage dans le milieu d'indice $n_2$.

On peut définir les angles __orientés__ pour chaque rayon:

* __angle incident__ $i_1$: de la normale vers le rayon incident.
* __angle réfléchi__ $r$:  de la normale vers le rayon réfléchi.
* __angle réfracté__ $i_2$:  de la normale vers le rayon réfracté.

```{figure} ./images/optique_descartes_plus_refringent.jpg
:name: descartes
:align: center
```
On a alors les relations géométriques suivantes:

\begin{align*}
r &= - i_1\\
n_1 \sin i_1 &= n_2 \sin i_2
\end{align*}
````

````{sidebar} Complément - Séparation énergétique
La loi de Snell-Descartes permet d'étudier géométriquement l'existence des deux rayons. Mais il faut préciser qu'il s'opère un division de l'énergie entre deux parts (transmise et réfléchie) __qui ne sont pas forcément égales__.

Le théorie électromagnétique (HP) permet de prévoir la répartition énergétique. On retiendra simplement qu'il n'y a pas séparation en deux parts égales et que celle-ci peut varier en fonction de l'angle d'incidence (dans certaines conditions, on peut même annuler la puissance réfléchie ou la puissance transmise).
````
