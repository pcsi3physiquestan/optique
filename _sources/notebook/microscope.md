---
jupytext:
  encoding: '# -*- coding: utf-8 -*-'
  formats: ipynb,md:myst
  split_at_heading: true
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3 (ipykernel)
  language: python
  name: python3
---

# Numérique : Systèmes optiques multilentilles
## Position du problème
On considère un microscope constitué :
* d'un objectif réalisé par une lentille mince de distance focale $f_{obj} = 4mm$ placé au point O.
* d'un oculaire dit de Ramsden constitué de deux lentilles minces de même distance focale de distance focale $f_2 = f_3 = 3cm$ distantes de $\overline{O_2 O_3} = {2 \over 3}f_3$
* la distance entre l'objectif et la première lentille de l'oculaire est $\Delta = 18cm$ (on l'appellera _intervale optique_).

Le but de l'exercice est de trouver par simulation numérique, puis par le calcul où placer un objet (de taille 1(unité arbitraire)) pour que l'image finale soit à l'infini.

On place l'origine de l'axe optique à l'emplacement de l'objectif et on suppose que le systèmes vérifient les conditions de Gauss.

## Modélisation sous Python
* On va modéliser un objet (ou une image) par une liste de deux éléments `[x, d]` correspondant à sa position $x$ sur l'axe optique et sa taille transverse $d$.
    * Dans la suite, si on utilise comme argument d'une fonction un objet lumineux (donc une liste de deux éléments), il sera appelé `obj` ou `obj1, obj2, ...`.
* On va modéliser une lentille mince par une liste de deux éléments `[x, f]` correspondant à sa position $x$ sur l'axe optique de son centre optique et sa distance focale image $f'$.
    * Dans la suite, si on utilie comme arguments d'une fonction une lentille (donc une liste de deux éléments), il sera appelé `L` ou `L1, L2, ...`.

> __Exercice :__  
> 1. Comment appelle-t-on le point sur l'axe optique où doit être placé l'objet?
> 2. Ecrire une fonction `image(L, obj)` qui renvoie les caractéristiques d'une image (liste à deux éléments) d'un objet `obj` par une lentille `L`.
> 3. Ecrire une fonction `microscope(fobj, f2, Delta, obj)` qui renvoie les caractéristiques d'une image (liste à deux éléments) d'un objet `obj` par un microscope dont la focale de l'objectif est `fobj`, celle des lentilles de l'oculaire `f2` (on rappelle qu'il y en a deux) et l'intervale optique `Delta`
> 4. Pour des objets situé entre l'objectif et 2cm en amont de l'objectif, tracer deux graphiques donnant l'un la position de l'image finale en fonction de la position de l'objet et la taille de l'image finale en fonction de la taille de l'objet. En déduire visuellement où placer l'objet. (Ne pas hésiter à "zoomer").
> 5. \*Pour déterminer numériquement la position de l'objet, réaliser une recherche de 0 (par dichotomie à $10^{-6} cm$ près sur la position de l'objet) sur la fonction $Y(x_{obj}$ où $x_{obj}$ est la position de l'objet et $Y$ l'inverse de la position de l'image.
> 6. Déterminer analytiquement la position de l'objet en déterminant successivement : la position du foyer principal objet de l'oculaire seule puis la position de l'objet.

_Indications utiles_ :
* Attention à ne pas confondre la position absolue sur un axe et une distance relative entre deux éléments.
* Il faudra peut-être tracer $Y(x_{obj})$ pour choisir l'intervalle pour la dichotomie.

```{code-cell} ipython3

```
