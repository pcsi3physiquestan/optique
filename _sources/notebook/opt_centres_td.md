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
# Entrainement : Systèmes centrés

Ces exercices seront traités en classe.

## Le sextant

Le sextant est un appareil qui était utilisé par les marins pour déterminer la latitude. Pour cela, il mesurait la hauteur d'un astre (Soleil,Lune... ) au dessus de l'horizon. Le sextant est composé de deux miroirs plans $M_1$ et $M_2$ (ce dernier étant semi-réfléchissant) et d'une lunette de visée (que nous n'étudierons pas ici). La direction OC du plan du miroir pointe un repère sur l'arc de cercle gradué AB qui mesure $60^{\circ}$. Sur la figure, les proportions ne sont pas respectées.

```{figure} ./images/sextant.jpg
:name: sextant
:align: center
:width: 75%
Sextant
```

Avec la lunette, l'observateur vise l'horizon donc l'axe optique de la lunette a la direction horizontale. La normale au plan du miroir $M_2$ est fixe et fait un angle de $30^{\circ}$. Ce miroir est aussi parallèle à la direction OA où O est le point d'incidence des rayons de l'astre sur le miroir $M_1$ (qu'on peut assimiler au "centre" du miroir plan $M_1$). On note $\theta$ l'angle entre la normale à $M_1$ et l'horizontale et $\phi$ celui de la direction de l'astre par rapport à l'horizontale. On les considère positifs dans la configuration donnée sur le schéma.


````{admonition} Exercice 
:class: attention

1. Déterminer en fonction de $\phi$ et $\theta$, l'angle $\alpha$ que fait le rayon réfléchi sur $M_2$ avec l'horizontale.
2. Quel doit-être l'angle $\theta$ pour que le rayon réfléchi sur $M_2$ soit selon l'axe optique de la lunette?
3. Dans ces conditions, déterminer la relation entre l'angle AOC et l'angle SOH où S désigne la position de l'astre et H l'horizon.
````

_Point utile pour cet exercice_
* _$\Longrightarrow$ [Miroir plan](miroir_plan)._
* _$\Longrightarrow$ Trigonométrie_

````{topic} Eléments de réponse (sans justification)
1. $2 \theta + \phi - \pi/3$
2. $\theta = \pi/6 - \phi / 2$
3. $\phi/2$
````

## Dioptre hémisphérique
On étudie un dioptre hémisphérique (une lentille) de rayon R et d'indice n plongé dans l'air d'indice 1. On s'intéresse aux phénomène d'aberration. Un faisceau cylindrique (de rayon $d_{\max}$) de lumière monochromatique arrive sous incidence normale sur la lentille; ce faisceau est donc issu d'un point objet B situé à l'infini dans la direction de l'axe.

```{figure} ./images/dioptre_hemispherique.jpg
:name: dioptre_hemi
:align: center
:width: 75%
```


````{admonition} Exercice 
:class: attention

1. On considère un rayon du faisceau de lumière à une distance d de l'axe optique. Établir la relation donnant CA en fonction de R = CS, et des angles i et r.
2. Montrer que quand on se place dans l'approximation de Gauss ($d \ll R$), on peut considérer que tous les rayons coupent l'axe optique en un même point F' dont on déterminer la distance à C. F' est donc l'image de B dans les conditions de Gauss.
3. Comment appelle-t-on F'?
4. On n'est plus dans les conditions de Gauss. Quelle est la valeur $d_0$ limite de d max du faisceau incident si l'on veut que tous les rayons du faisceau incident ressortent de la lentille?
5. Faire l'application numérique pour n = 1,5, R = 5cm.
6. \*Faire un développement limité au second ordre en i de la distance CA. Conclure quant à la possibilité de réaliser l'approximation de Gauss.
````
_Point utile pour cet exercice_
* _$\Longrightarrow$ [Lois de Snell-Descartes](snell_enonce)._
* _$\Longrightarrow$ [Réflexion totale](snell_totale)._
* _$\Longrightarrow$ [Eléments principaux d'un système centré](foyers)._
* _$\Longrightarrow$ [Méthode : Recherche d'un foyer](meth_foyer)._
* _$\Longrightarrow$ Trigonométrie_

````{topic} Eléments de réponse (sans justification)
1. $CA = R \cos i + R \frac{\sin i}{\tan(r - i)}$
2. $CF' = R \frac{n}{n-1}$
3. Foyer principal image
4. $d_0 = R / n$
5. 3 cm
6. $CA = CF' - \frac{d^2}{2R}$
````