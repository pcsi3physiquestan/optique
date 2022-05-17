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

# Zones d'espaces conjuguées
On veut ici relier des zones d'espaces dans lesquelles l'objet et l'image conjugué seront du même type: par exemple une zone où l'on aura toujours un objet réel donnant une image virtuelle (attention la zone de l'objet ne sera pas la même que la zone de l'image.


````{admonition} Exercice 
:class: attention

On considère une lentille convergente. Déterminer les zones objets correspondant aux configuration suivantes:

1. l'objet est réel et l'image est virtuelle.
2. l'objet est réel et l'image est réelle.
3. l'objet est virtuel et l'image est virtuelle.
4. l'objet est virtuel et l'image est réelle.

Dans chaque configuration, on déterminera aussi:

*  la zone image correspondante
* si l'image est droite ou renversée
* si l'image est grandit, rétrécie ou si elle peut-être les deux.

Reprendre le même exercice pour une lentille divergente.
````

````{important} Bilan à retenir - Ce n'est PAS la correction., dropdown
On retiendra que pour un lentille convergente, on peut obtenir les 3 configurations suivantes:

* objet réel avant le foyer objet et image réelle après le foyer image. L'image est alors renversée et elle peut être agrandie ou rétrécie.
* objet réel entre F et O et image virtuelle. L'image est droite et toujours plus grande que l'objet.
* objet virtuel et image réelle entre O et F'. L'image est droite et toujours plus petite que l'objet.
````

````{important} Bilan à retenir - Ce n'est PAS la correction., dropdown

On retiendra que pour un lentille divergente, on peut obtenir les 3 configurations suivantes:

* objet réel et image virtuelle entre F' et O. L'image est alors droite et elle est toujours plus petite que l'objet.
* objet virtuel entre O et F et image réelle. L'image est droite et toujours plus grande que l'objet.
* objet virtuel après F et image virtuelle avant F'. L'image est renversée et elle peut être agrandie ou rétrécie.
````


```{figure} ./images/optique_espaces_conjugues.jpg
:name: espaces_conjugues
:align: center
Les couleurs donnent la correspondance entre les zones objets et images
```


````{dropdown} Remarque

__Points principaux__ On remarquera que les points qui délimitent les zones d'espaces conjugués sont des points importants pour l'objet (l'infini, le foyer __objet__, le centre optique) ou pour l'image (l'infini, le foyer __image__, le centre optique).
````


````{admonition} Tracé graphique
:class: hint, dropdown
Il est __très vivement__ conseillé de s'entraîner à déterminer l'image d'un point objet dans chaque zone objet pour chaque type de lentille puis de faire l'inverse: déterminer l'antécédent d'un point image dans chaque zone image pour chaque type de lentille.

Vous serez alors à même de vous débrouiller dans chaque situation.
````