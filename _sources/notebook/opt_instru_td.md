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
# Entrainement : Instruments d'optique

Pensez à travailler les [questions de cours](https://moodlecpge.stanislas.fr/mod/resource/view.php?id=127) et les [raisonnements qualitatifs](https://moodlecpge.stanislas.fr/mod/quiz/view.php?id=128) (en ligne) aussi.

Il est vivement conseillé de s'entraîner aussi avec le devoir libre sur l'appareil photographique.

## Le microscope
Un microscope optique permet d'observer des globules sanguins. Il est modélisable par deux lentilles minces convergentes $L_1$ pour l'objectif de distance focale $f_1$ et $L_2$ pour l'oculaire de distance focale $f_2$. Il est réglé pour donner une image à l'infini d'un objet réel $AB$ perpendiculaire à l'axe optique (A étant sur l'axe optique) légèrement en avant du foyer objet de l'objectif. Cette image est observée par un oeil emmétrope (normal) placé au voisinage du foyer image de l'oculaire. On notera $A'B'$ l'image intermédiaire. Le microscope porte les indications suivantes:

* $\times 40$ pour l'objectif, ce qui signifie que la valeur absolue du grandissement de l'objet $AB$ par l'objectif est de 40
* $\times 10$ pour l'oculaire, ce qui signifie que le grossissement commercial ou rapport entre l'angle sous lequel on voit l'image à l'infini d'un objet à travers l'oculaire seul et l'angle sous lequel on voit ce même objet à l'oeil nu lorsqu'il est situé à la distance minimale de vision distincte $\delta=-25\rm{cm}$ vaut 10.
* $n\sin u =\omega_0=0,65$ pour l'ouverture numérique ou la valeur de $n\sin(u)$ avec n le milieu dans lequel se trouve l'objectif et u l'angle maximum des rayons issus de A arrivant sur l'objectif.
* $\Delta=16\rm{cm}$ pour l'intervalle optique ou distance entre le foyer image $F'_1$ de l'objectif et le foyer objet $F_2$ de l'oculaire.


````{admonition} Exercice 
:class: attention
1. Faire un schéma du dispositif (sans respecter les échelles) et tracer la marche de deux rayons lumineux issus du point B de l'objet $AB$, l'un émis parallèlement à l'axe optique et l'autre passant par le foyer objet de l'objectif.
2. En utilisant le grossissement commercial, déterminer la distance focale $f_2$ de l'oculaire.
3. Déterminer la distance focale $f_1$ de l'objectif. On pourra utiliser le grandissement de l'objectif.
4. Calculer la distance $\overline{O_1 A}$ permettant de positionner l'objet.
5. Déterminer la latitude de mise au point à savoir la variation de la distance $\rm{O_1 A}$ compatible avec l'observation d'une image par l'oeil situé au foyer image de l'oculaire.
6. Calculer le grossissement commercial du microscope pour une image finale à l'infini.
7. Calculer l'angle u intervenant dans l'ouverture numérique pour un objectif placé dans l'air. Le microscope utilisé est-il utilisé dans les conditions de Gauss? Quel type d'aberrations doit-on corriger? Quel est l'ordre de grandeur du diamètre de la monture de l'objectif?
8. Déterminer la position et la taille du cercle oculaire défini comme l'image de la monture de l'objectif à travers l'oculaire. Quel est l'intérêt de placer l'oeil dans le plan du cercle oculaire?
````

_Point utile pour cet exercice_
* _$\Longrightarrow$ [Méthode : Tracés graphiques](traces_gr)._
* _$\Longrightarrow$ [Méthode : Etude qualitative](lentille_qu)._
* _$\Longrightarrow$ [Relations de conjugaison](conjugaison)._
* _$\Longrightarrow$ [Eléments principaux d'un système centré](foyers)._
* _$\Longrightarrow$ [Détermination d'un grossissement](grossissement)._


````{dropdown} Correction partielle

Corrigé des dernières questions (7 et 8).

* Dans l'air $n \approx 1$ donc $u = \arcsin \omega_0 = 0.71 \rm{rad} = 41 ^{\circ}$. Le microscope n'est donc pas utilisé dans les conditions de Gauss (en pratique, les lentilles sont taillées pour atténuer les aberrations géométriques et l'utilisation d'un ensemble de lentilles corrige aussi les aberratinos chromatiques). Il vient: $D = \overline{O_1 A} \tan \arcsin u = $ (remplacer $\overline{O_1 A}$ par l'expression trouvée précédemment).
* $\overline{F'_2 O_c} = \frac{(\delta / G_c)^2}{\Delta + \Delta / \gamma}$ et $D_{Oc} = -D \times \frac{(\delta / G_c)}{\Delta + \Delta / \gamma}$ grâce à la relation de grandissement au foyer image (le diamètre est donné en valeur absolue ici).
````