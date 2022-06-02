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

# Lentilles minces: tracés des rayons

## Rayons utiles
````{topic} Mise en contexte
En optique, les études graphiques peuvent être très utiles pour raisonner et prévoir. Mais pour une lentille mince, l'utilisation de la schématisation de Gauss empêche l'utilisation des lois de Snell-Descartes (il n'y a plus la courbure du dioptre ni son épaisseur).

On doit donc utiliser d'autres méthodes pour construire la position d'une image A'B' connaissant l'objet AB, construire la position d'un objet AB connaissant la position de l'image, déterminer le devenir d'un rayon ou d'un faisceau... 
````

Nous allons présenter ici les 4 rayons (plutôt 3 rayons et une propriété particulière) qui peuvent être utiles pour les études présentées ci-dessus. Ils utilisent les éléments principaux de la lentille.


````{important} __Fondamental : Rayons utiles__
* Un rayon incident parallèle à l'axe optique ressort en passant par le foyer principal image.

_A l'inverse, un rayon sortant passant par le foyer principal image a pour antécédent un rayon parallèle à l'axe optique._
```{figure} ./images/optique_rayon_entrant_para.jpg
:name: l_rayon_entrant
:align: center
:width: 40%
```

* Un rayon entrant passant par le foyer principal objet ressort de la lentille parallèlement à l'axe optique.

_A l'inverse, un rayon sortant parallèle à l'axe optique a pour antécédent un rayon qui passe par le foyer principal objet._
```{figure} ./images/optique_rayon_sortant_para.jpg
:name: l_rayon_sortant
:align: center
:width: 40%
```


* Un rayon entrant passant par le centre optique ressort non dévié.
```{figure} ./images/optique_rayon_centre_optique.jpg
:name: l_rayon_centre
:align: center
:width: 40%
```

* Deux (ou plus) rayons incidents parallèles entre eux ressortent en se croisant en un foyer image (secondaire ou principal) donc dans le plan focal image.
```{figure} ./images/optique_rayon_faisceau_parallele.jpg
:name: l_faisceau
:align: center
:width: 40%
```

* Deux (ou plus) rayons transmis parallèles entre eux ont pour antécédents des rayons qui se croisent en un foyer objet (secondaire ou principal) donc dans le plan focal objet.
````

