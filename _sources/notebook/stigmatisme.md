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


````{topic} Besoin de netteté
Le but d'utilisation d'un système optique est de pouvoir observer une image nette et non déformée à travers l'instrument.

En terme de faisceau lumineux, celà implique que pour un faisceau incident issu d'un point objet traversant le système optique, le faisceau sortant doit concourir en un point.

Ci dessous l'exemple du miroir plan où le faisceau issu du point $A_1$ donne un faisceau réfléchi qui concourt au point $A_2$ (plus précisément c'est le prolongement des rayons réfléchies réels qui concourent en $A_2$).

```{figure} ./images/optique_miroir_plan.jpg
:name: miroir_plan_1
:align: center
```
````

````{important} __Stigmatisme rigoureux__
:class: full-width

Un système optique est dit __rigoureusement stigmatique__ pour deux points (A ;A') si l'ensemble des rayons lumineux issus du premier point A et traversant le système forment d'autres rayons lumineux dont les supports passent par le second point A'.

Le premier point A est appelé __point objet__, le second __point image A'__. On dit que les deux points A et A' sont __conjugués__.

```{figure} ./images/objet_image_p.jpg
:name: objet_p
:align: center
Conjugaison d'un point objet et image
```

```{margin}
On parlera par extension d'une image étendue, ensemble de points image conjuguées aux points objets d'un objet éntendu.
```
````

## Images réelles et virtuelles

````{important} __Image réelles et virtuelles__
:class: full-width
* Lorsque le point image est au concours des rayons réels, on dit que l'__image est réelle__ (comme $A'_1$ dans l'[image ci-après](image_virtuelle)). _En pratique, il s'agit d'une image formée en aval du système optique. On peut y placer un écran et observer l'image sur l'écran._
* Lorsque le point image est au concours du prolongement virtuels des rayons sortants (rayons sortants dits virtuels), on dit que l'__image est virtuelle__ (comme $A'_2$ sur l'[image ci-après](image virtuelle) ou $A_2$, image de $A_1$ dans le cas du [miroir plan ci-dessus](miroir_plan_1)). En pratique, il s'agit d'une image formée avant la sortie du système optique. On ne peut la matérialiser sur un écran _mais il suffit de placer son oeil derrière le système optique pour la voir_.

```{figure} ./images/optique_image_virtuelle_reelle.jpg
:name: image_virtuelle
:align: center
```
````

````{topic} Observation d'une image
```{attention}
L'image est ce qu'on voit en plaçant notre oeil après le système optique (à condition de se placer évidemment derrière l'endroit où se forme l'image !).

On peut voir l'image à travers un système optique quelque soit la nature (réelle ou virtuelle) de l'image.

Le caractère virtuel de l'image empêche simplement de placer un écran pour qu'elle se forme sur celui-ci.
```
````

