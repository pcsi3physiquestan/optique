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

# Eléments principaux des systèmes centrés

## Eléments principaux: foyers

```{margin}
* La définition avec les rayons est utiles pour les graphiques
* La définition en terme de conjugaison est utile pour les mise en équation
```
````{important} __Foyers principaux objets et images__
* On définit le __foyer principal objet__ comme le point où tout rayon _incident_ passant par le foyer principal objet ressort du système optique (__rayon transmis__) en étant parallèle à l'axe optique.

__Le foyer principal objet est donc l'antécédent du point à l'infini sur l'axe optique.__

* On définit le foyer principal image comme le point tel que tout rayon __incident__ parallèle à l'axe optique ressort du système optique (__rayon transmis)__ en passant par le foyer principal image.

__Le foyer principal image est donc l'image du point à l'infini sur l'axe optique.__

```{figure} ./images/optique_foyer_quelconque.jpg
:name: foyer_principal_image_objet
:align: center
Foyer principal image (gauche) et objet (droite)
```

* Les plans focaux objet et image sont respectivement les plans frontaux contenant les foyers principaux objet ou image.
````

```{sidebar} Objet et image à l'infini
* Il est fondamental de savoir reconnaître et représenter un objet ou une image à l'infin : ils ne sont pas représentés par des points mais par des faisceaux parallèles dont _l'angle par rapport à l'axe optique défini la position de l'objet/image à l'infini. On parle __d'angle sous lequel et vu l'objet__.
```
````{important} __Foyers secondaires objets et images, dropdown__
Les foyers _secondaires_ objet et image sont les points respectivement du plan focal objet ou image n'étant pas sur l'axe optique.

* Un foyer secondaire objet a pour image un point à l'infini __hors de l'axe optique__ (qu'on peut représenter par un faisceau sortant parallèle entre eux mais non parallèle à l'axe optique). _Une telle image est caractérisée par l'angle du faisceau ainsi formé_.

* Un foyer secondaire image a pour antécédent un point à l'infini __hors de l'axe optique__ (qu'on peut représenter par un faisceau entrant parallèle entre eux mais non parallèle à l'axe optique). _Un tel objet est caractérisé par l'angle du faisceau ainsi formé_.
````

## Eléments principaux: Centre optique et distance focale

```{margin} Remarque : Existence du centre optique
Pour un système optique quelconque, le centre optique n'existe pas forcément. Par exemple pour un système à plusieurs lentilles (lunette astronomique... ), il n'y a pas de centre optique du système complet.
```
````{important} __Centre optique__
Le __centre optique__ est le point de l'axe optique où tout rayon incident pointant vers ce point ressort sans être dévié.
````

```{margin}
Attention aux appelations et aux notations. Il arrive qu'on trouve la notation f pour la distance focale image.

De plus, on parle souvent - par abus de langage - de distance focale pour désigner implicitement la distance focale image.
```
````{important} __Distance focale objet et image__
* Lorsque le centre optique existe, on définit la distance focale objet f comme la distance __algébrique__ entre le centre optique O et le foyer principal objet F: $f = \overline{OF}$
* Lorsque le centre optique existe, on définit la distance focale image f' comme la distance __algébrique__ entre le centre optique O et le foyer principal image F': $f' = \overline{OF'}$
* On définit la vergence $V = 1 / f'$ avec $f'$ la distance focale image. Son unité est la __dioptrie__ notée $\delta$
````


## Exemple: Détermination du foyer image d'un miroir sphérique.

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
````{admonition} A retenir
* L'utilisation de la géométrie et de la trigonométrie pour établir de relations mathématiques
* L'utilisation des petits angles pour se placer dans les conditions de gauss
* Dans les conditions de Gauss (ordre 1), on trouve normalement un résultat dépendant de la position de l'objet/image mais _pas du rayon choisi (ici de l'angle i)._ C'est le __stigmatisme approchée.__
````