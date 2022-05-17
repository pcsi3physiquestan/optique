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
# Stigmatisme rigoureux. Notion d'images.

Un système optique sert à modifier la position et la taille apparente de l'objet lumineux visé. Son correspondant - son conjugué - après le système optique (ce qu'on va voir à travers la jumelle, la lunette, la loupe... ) est appelé __image__ et celle-ci doit être vue nettement. C'est-à-dire qu'à un point de l'objet doit correspondre dans l'image...  un point (et non une tâche). C'est ce qu'on appelle le __stigmatisme.__

Nous allons simplement présenter ici la définition du stigmatisme et dans le cadre où ce dernier est réalisé, préciser la notion d'image.

## Stigmatisme rigoureux


````{dropdown} Besoin de netteté
Le but d'utilisation d'un système optique est de pouvoir observer une image nette et non déformée à travers l'instrument.

En terme de faisceau lumineux, celà implique que pour un faisceau incident issu d'un point objet traversant le système optique, le faisceau sortant doit concourir en un point.

Ci dessous l'exemple du miroir plan où le faisceau issu du point $A_1$ donne un faisceau réfléchi qui concourt au point $A_2$ (plus précisément c'est le prolongement des rayons réfléchies réels qui concourent en $A_2$).

```{figure} ./images/optique_miroir_plan.jpg
:name: miroir_plan_1
:align: center
```
````

````{important} __Définition : Stigmatisme rigoureux__

Un système optique est dit __rigoureusement stigmatique__ pour deux points (A ;A') si l'ensemble des rayons lumineux issus du premier point A et traversant le système forment d'autres rayons lumineux dont les supports passent par le second point A'.

Le premier point A est appelé point objet, le second point image A'. On dit que les deux points A et A' sont conjugués.
````

## Images réelles et virtuelles

````{important} __Définition : Image ponctuelle__

Lorsque le stigmatisme est réalisé, le faisceau incident issu d'un point objet A ressort du système optique en concourant en un point $A_1$ appelé image de l'objet __$A_1$__.

On dit que A et $A_1$ sont __conjugués.__

On parlera par extension de l'image d'un objet étendu.
````

````{important} __Définition : Image réelles et virtuelles.__

Lorsque le point image est au concours des rayons réels, on dit que l'image est réelle (comme $A'_1$ dans l'image ci-dessous). En pratique, il s'agit d'une image formée en aval du système optique. On peut y placer un écran et observer l'image sur l'écran.

Lorsque le point image est au concours du prolongement virtuels des rayons sortants (rayons sortants dits virtuels), on dit que l'image est virtuelle (comme $A'_2)$. En pratique, il s'agit d'une image formée avant la sortie du système optique. On ne peut la matérialiser sur un écran mais il suffit de placer son oeil derrière le système optique pour la voir.

```{figure} ./images/optique_image_virtuelle_reelle.jpg
:name: image_virtuelle
:align: center
```
````

````{attention}
:class: dropdown
__Observation d'une image__

L'image est ce qu'on voit en plaçant notre oeil après le système optique (à condition de se placer évidemment derrière l'endroit où se forme l'image !).

On peut voir l'image à travers un système optique quelque soit la nature (réelle ou virtuelle) de l'image.

Le caractère virtuel de l'image empêche simplement de placer un écran pour qu'elle se forme sur celui-ci.
````

