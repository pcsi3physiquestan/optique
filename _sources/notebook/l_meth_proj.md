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

# Projection

Nous allons étudier ici les conditions de projection, c'est-à-dire les conditions permettant de projeter un objet sur un écran à une distance donnée. On retrouve évidemment ce principe dans tous les dispositifs...  de projection comme un vidéo-projecteur.

On désire projeter un objet lumineux (exemple l'objet illumé par un vidéoprojecteur) sur un écran situé à une distance D (par exemple le tableau). On dispose pour celà de lentilles et on veut savoir quelles sont les lentilles qu'on peut choisir pour réaliser cette projection.

On s'impose que:
* Condition 1: l'image sur l'écran doit être nette (!)
* Condition 2: l'image sur l'écran doit être grandie.

````{admonition} Exercice 
:class: attention

1. Analyse de la condition 1:
    1. Quel est la nature (réel/virtuel) de l'objet ? de l'image ? Quelle type de lentille faut-il choisir?
    2. Justifier que la distance focale f' de la lentille doit vérifier la __condition de projection__ : $D > 4f'$
2. Analyse de la condition 2:
	1. La condition de projection étant réalisée, déterminer les distances $\overline{OA}$ entre la lentille et l'objet et $\overline{OA'}$ entre la lentille et l'écran en fonction de D et f'. Vous devez trouver deux possibilités.
	2. Laquelle de ces deux possibilités permet de satisfaire la condition 2?
	3. Exprimer dans ces conditions le grandissement.
	4. Estimer la distance focale de la lentille du vidéoprojecteur de la classe ainsi que le grandissement.
	5. Comment faut-il choisir la distance focale pour obtenir un grossissement important. Quel problème celà peut-il poser?
````

````{dropdown} Correction
 

````{admonition} Bilan à retenir - Ce n'est PAS la correction.
:class: important, dropdown

On retiendra que:
* pour pouvoir projeter un objet sur un écran situé à une distance D, il faut __une lentille convergente__ dont la distance focale satisfait __la condition de projection__ $D > 4f'$__
* pour grandir l'objet, la lentille doit se trouver plus proche de l'objet que de l'écran.
````
