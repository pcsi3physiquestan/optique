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

# Lentilles minces: Présentation

## Lentilles minces: définition

````{important} __Lentille sphérique mince__

Une lentille sphérique est un système optique centré composé d'un milieu transparent taillé suivant deux dioptres sphériques. On a repéré ici les centres et sommets respectifs des deux faces: $C_1, C_2, S_1$ et $S_2$.

```{figure} ./images/optique_lentille_principe.jpg
:name: lentille_principe
:align: center
```
Soit e l'épaisseur de la lentille $e = \overline{S_1 S_2}$, on dit que la lentille est mince si $e \ll C_1 S_1;  e \ll C_2 S_2;  e \ll C_1 C_2$

Dans ces conditions, on peut confondre les sommets $S_1$ et $S_2$. Ce point sera, dans le cadre d'application des conditions de Gauss, le __centre optique__ de la lentille.
````

## Lentilles minces: typologie

````{sidebar} Remarque

Comportement des faisceaux qui traversent chaque lentille.

* lentille convergente: l'ouverture angulaire du faisceau tend à diminuer.
* lentille divergente: l'ouverture angulaire du faisceau tend à augmenter.

```{figure} ./images/optique_lentille_cv_dv.jpg
:name: lentille_cvdv
:align: center
:width: 75%
```
````
````{important} __Lentilles divergente et convergente__

* Si la distance focale image est positive, on dit que la lentille est __convergente__.
* Si la distance focale image est négative, on dit que la lentille est __divergente__.
````


## Lentilles minces: Schématisation de Gauss

````{margin} Stigmatisme approché
Dans le cadre des conditions de Gauss, une lentille mince réalise un stigmatisme approché.
````

````{important}
:class: full-width
__Schématisation de Gauss d'une lentille convergente__

```{figure} ./images/optique_gauss_convergente.jpg
:name: gauss_cv
:align: center
:width: 40%
Schématisation de Gauss (CV)
```

Dans le cadre des conditions de Gauss, on schématise une lentille mince convergente sous la forme ci-contre.

```{figure} ./images/optique_gauss_divergente.jpg
:name: gauss_dv
:align: center
:width: 40%
Schématisation de Gauss (DV)
```

Dans le cadre des conditions de Gauss, on schématise une lentille mince divergente sous la forme ci-contre.
````

