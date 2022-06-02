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

# Etude d'une lunette afocale

On considère un lunette afocale, c'est-à-dire donnant une image à l'infini d'un objet à l'infini. Nous allons voir quelques caractéristiques et méthodes d'étude d'un tel dispositif.

On considère une lunette constituée de deux lentilles:
* l'objectif $L_1$ (de distance focale image $f_1$). Il sert à grandir un objet et recueillir un maximum de de lumière de l'objet
* l'oculaire $L_2$ (de distance focale image $f_2$). Il sert - comme on l'a vu précédemment - à grossir l'image intermédiaire donnée par l'objectif et à la renvoyer au Punctum Remotum de l’oeil pour limiter la fatigue oculaire.

_S'y ajoute en général un __réticule__ entre l'objectif et l'oculaire où doit - lorsque la lunette est réglée - venir se former l'image intermédiaire. Il sert au réglage de la lunette et peut-être gradué pour réaliser des mesures sur l'objet (ou plus précisément l'image intermédiaire)._

Pour les constructions géométriques et les applications numériques, on prendra:

* $f_1 = 5\rm{cm}$ et $f_2 = 2 \rm{cm}$.
* Distance entre les centre optique: $\overline{O_1 O_2} = d > 0$.
* Diamètre l'objectif: $D_1 = 4 \rm{cm}$
* Diamètre l'oculaire: $D_2 = 2 \rm{cm}$

On notera les foyers objets et images respectivement $F_1, F_2$ et $F_1, F_2$.

On notera A un objet à l'infini sur l'axe optique, $A'$ son image par l'objectif (image intermédiaire) et $A_1$ son image finale

On notera B un objet à l'infini hors de l'axe optique, $B'$ son image par l'objectif (image intermédiaire) et $B_1$ son image finale


````{admonition} Exercice - Généralités et grossissement
:class: attention
1. Une lunette est dite __afocale__ si elle donne d'un objet à l'infini une image à l'infini. Pourquoi dit-on qu'elle est __afocale__?
2. En déduire une expression de $d$ en fonction de $f_1$ et $f_2$. Calculer $d$ avec les valeurs données dans le tableau. On gardera cette valeur pour $d$ dans toute la suite de l'exercice.
3. Faire un schéma de la lunette astronomique (on prendra une échelle de 1:1 pour les dimensions longitudinales et transversales). Tracer le parcours de rayons arrivant d'un point B situé à l'infini hors de l'axe optique. On notera l'angle des rayons incidents avec l'axe optique $\theta$.On notera l'angle des rayons transmis par le système avec l'axe $\theta'$.
4. Définir le grossissement G de la lunette astronomique. Donner son expression en fonction des distances focales des lentilles. Calculer G.
5. Proposer deux façon d'augmenter le grossissement G. Quels sont les contraintes qui empêchent de l'augmenter indéfiniment?
6. L'image observée par l'oeil est-elle droite ou inversée? 
7. Déterminer la taille de l'image intermédiaire $\overline{A'B'}$.
````

````{important} 
:class: dropdown
__Bilan à retenir - Ce n'est PAS la correction.__

* Un dispositif __afocale__ donne une image à l'infini d'un objet à l'infini. Les foyers sont alors renvoyés à l'infini (il n'y a pas de foyers).
* Pour le calcul du grossissement, il est crucial de passer par l'image intermédiaire. On ne calcule pas ici de grossissement commercial puisqu'on ne peut se rapprocher d'un objet à l'infini !
````

````{admonition} Exercice - Cercle oculaire
:class: attention
On appelle cercle oculaire l'image de la lentille $L_1$ par la lentille $L_2$.

1. Déterminer la position et la taille du cercle oculaire. Donner leur valeur numérique.
2. Justifier l'affirmation suivante "Tout rayon entrant dans la lunette (et en ressortant évidemment) passe à l'intérieur du cercle oculaire". En déduire que le cercle oculaire est l'endroit idéal pour placer son oeil.
3. Faire un schéma permettant de construire le cercle oculaire.
````

````{important} 
:class: dropdown
__Bilan à retenir - Ce n'est PAS la correction.__

Le cercle oculaire - image de l'objectif par l'oculaire - est l'endroit où passe toute la lumière entrante dans un espace étroit. C'est le meilleur endroit où placer son oeil pour avoir un maximum de luminosité et de champ.

En général, les appareil sont construits de sorte que le cercle oculaire soit très proche de l'oculaire (ce qui revient à prendre une $f_2$ très petite.
````

````{admonition} Exercice - Limite de résolution
:class: attention
On suppose dans un premier temps que la résolution de la lunette est due au pouvoir séparateur de l'oeil. On rappelle que le pouvoir séparateur de l'oeil est $\theta'_m=3.10^{-4}\rm{rad}$.

1. Déterminer la résolution angulaire de la lunette étudiée ici.
2. Pour des étoiles lointaines quasi-ponctuelles, quel autre phénomène risque de gêner leur observation?
````

````{admonition} Exercice - Latitude de mise au point
:class: attention
1. L'oeil accommodant, l'objet visé peut ne pas être strictement à l'infini. Rappeler ce qu'est le processus d'accommodation.
2. Déterminer la position $A_1$ de l'image finale d'un objet réel visé situé en un point A qui n'est pas à l'infini. On exprimera la distance $\overline{F_2 A_1}$ en fonction de $\overline{F_1 A}$.
3. L'observateur place son oeil sur le cercle oculaire. Déterminer la latitude de mise au point.
````

````{admonition} Exercice - Lunette réelle
:class: attention
On s'intéresse à une lunette réelle. Ses caractéristiques sont:
* Distance focale: 600 mm.
* Diamètre de l'objectif: 50 mm.
* Oculaires: 4 mm.
* Diamètre oculaires: 24,5 mm.
* Grossissement: $150 \times$.

1. Vérifier le grossissement annoncé.
2. Déterminer le champ en pleine lumière pour cette lunette astronomique.
3. Observe-t-on la lune en entier?
4. Quelle est la taille du plus petit cratère lunaire qu'on peut observer avec une telle lunette.
````

````{admonition} Aller plus loin - Champ angulaire
:class: attention
1. Pour un objet situé à l'infini, quelle est le diamètre du faisceau incident?
2. Dans le cas d'un faisceau parallèle à l'axe optique, déterminer le diamètre du faisceau transmis. Faire un schéma représentant le faisceau et son passage à travers la lunette. Plus ce diamètre est grand, plus la lunette est lumineuse, c'est pourquoi, outre le grossissement, le diamètre de l'objectif est déterminant dans la qualité de la lunette.
3. Faire le même schéma pour un faisceau faisant un angle $\theta=30^{\circ}$ par rapport à l'axe optique. Que se passe-t-il? En déduire que le faisceau "utile" entrant, c'est-à-dire l'ensemble des rayons entrant dans la lunette qui ressortent effectivement dépend de l'angle. Quelle est la conséquence sur l'observation?
4. Déterminer graphiquement l'angle maximal pour lequel la section du faisceau "utile" est encore maximale (c'est-à-dire vaut la section déterminée pour le cas d'un faisceau parallèle à l'axe optique). On notera cette angle $\theta_{\max}$.

On appelle cet angle le champ (angulaire) de pleine lumière. Quand on observe le ciel, la faible luminosité empêche souvent de visualiser des objets qui ne sont pas dans le champ de pleine lumière (même si une partie de la lumière qui arrive jusqu'à la lunette en ressort).

On peut montrer que ce champ a pour expression: $\tan(\theta_{\max})=\frac{1}{2} \frac{D_2 f_1 - D_1 f_2}{f_1 (f_1+f_2)}$.
````
