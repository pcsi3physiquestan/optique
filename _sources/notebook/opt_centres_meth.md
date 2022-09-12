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

# Méthode : Recherche des éléments principaux
````{topic} Méthodes présentées
* L'utilisation de la géométrie et de la trigonométrie pour établir de relations mathématiques
* L'utilisation des petits angles pour se placer dans les conditions de gauss
* Dans les conditions de Gauss (ordre 1), on trouve normalement un résultat dépendant de la position de l'objet/image mais _pas du rayon choisi (ici de l'angle i)._ C'est le __stigmatisme approchée.__
````

## Foyer image d'un miroir sphérique.

````{admonition} Exercice 
:class: attention

On considère une portion de sphère de rayon R dont l'intérieur est entièrement réfléchissant.

1. On considère un rayon incident parallèle à l'axe optique à une distance d de ce dernier. Représenter graphiquement le rayon réfléchi et l'intersection entre ce rayon et l'axe optique. Comment appellerait-on ce point ?
2. Déterminer la distance (algébrique) entre le centre de la sphère miroir et le point d'intersection précédent.
3. Simplifier l'expression précédente pour d >> R. Commenter le résultat.

_La correction est en ligne._
````

````{topic} Correction
>__Q1.__ On utilise l'égalité de l'angle incident et de l'angle réfléchie (la normale à une sphère est son rayon).
>
```{figure} ./images/exo_miroir_foyer.png
:name: miroir_foyer
:align: center
:width: 50%
```
>
>Le point F est le point d'intersection de rayons sortant issus des rayons incidents parallèle à l'axe optique, il correspond donc à un bon candidat pour le foyer principal image.
>
>__Q2.__ Le rayon incident est parallèle à l'axe optique, il vient que l'angle entre le rayon CI et l'axe optique est aussi l'angle i et le triangle CIF est donc isocèle en F.  
On peut alors utiliser le produit scalaire:
>
>\begin{align*}
CI^2 &= \overrightarrow{CI} \cdot \overrightarrow{CI} = \left(\overrightarrow{CF} + \overrightarrow{FI}\right) \cdot \left(\overrightarrow{CF} + \overrightarrow{FI}\right) \\
&= CF^2 + IF^2 + 2 \overrightarrow{CF} \cdot \overrightarrow{FI} = 2 CF^2 + 2 CF^2 \cos {\left(\pi - (\pi - 2i) \right)} \\
&= 2 CF^2 \left(1 + \cos 2i\right)
\end{align*}
>
>Il vient:
>
>\begin{equation}
\boxed{CF = \frac{R}{2 \cos i}}
\end{equation}
>
>Remarque: On observe que la position du point dépend de l'angle et donc du rayon: on n'a pas de stigmatisme rigoureux.
>
>__Q3. Condition de Gauss__. Lorsque $d \ll R$, il vient que $i \ll 1$ donc $CF \approx \frac{R}{2}$
>
>Cette fois, la position du foyer ne dépend plus des rayons: en sélectionant les rayons paraxiaux (conditions de Gauss), on réalise un stigmatisme approché.
````