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
(oeil)=
# L'oeil et ses défauts

## Modélisation

### Eleménts et modélisation

````{topic} Eléments de l'oeil
D'un point de vue optique, on distingue plusieurs éléments de l'oeil (cette liste n'est pas exhaustive mais elle suffit à notre étude).

* _La rétine_: constituée des cellules rétiniennes et reliée au nerf optique (qui apporte les information au cerveau). C'est l'endroit où l'image doit se former nettement.
* _Le cristallin_: corps vitreux sur le devant de l'oeil. C'est "le système centré" qui sert à dévié les rayons pour former une image de l'objet visé sur la rétine.
* _La pupille_: devant le cristallin, elle joue le rôle de diaphragme, notamment pour éviter de saturer les cellules rétiniennes en lumière.

```{figure} ./images/optique_oeil_schema.jpg
:name: oeil_schema
:align: center
:width: 40%
```
````

````{important} __Modélisation optique de l'oeil__
:class: full-width
Du point de vue de l'optique géométrique, on peut modéliser l'oeil comme une lentille (le cristallin) diaphragmée (par la pupille) - celle-ci ne sera pas toujours représentée. La lentille est située en amont d'un écran (la rétine) situé à une distance d (en général $d \approx 2.5cm$) pour un oeil emmétrope - oeil normal).

```{figure} ./images/optique_oeil_modele.jpg
:name: oeil_modele
:align: center
:width: 40%
```
````

(oeil_acco)=
### Accomodation

```{sidebar} Accomodation et fatigue oculaire
Plus l'objet se rapproche de l'oeil, plus les muscles doivent bomber le cristallin ce qui occasionne une fatigue oculaire d'autant plus grande.
```
````{important} __Principe d'accomodation__
:class: full-width
Lorsque l'oeil vise un objet, il doit adapter sa distance focale pour former nettement l'image de l'objet visé sur la rétine. On parle __d'accomodation.__

L'accomodation de l'oeil se fait grâce à des muscles qui vont déformer le cristallin et __changer sa distance focale__.

* L'oeil ne peut voir plus loin qu'un point appelé __Punctum Remotum__. Lorsqu'il vise ce point, les muscles de l'oeil sont relâché et ne se fatiguent pas. On dit que __l'oeil est au repos__.
* L'oeil ne peut voir plus près qu'un point appelé __Punctum Proximum__ (car c'est la configuration où le cristallin est bombé au maximum).

````


````{admonition} Oeil emmétrope
:class: tip
L'oeil emmétrope ou oeil normal est considéré comme la norme lorsqu'il s'agit d'étudier un oeil (on parle aussi d'oeil sans défaut) ou de construire et d'évaluer un instrument d'optique (cf. suite). Ses caractéristiques sont les suivantes:

* Le punctum Remotum est à l'infini.
* Le punctum Proximum est à une distance $d \approx 25 cm$
````


````{topic} Défauts de l'oeil
Voici une présentation succincte des différents défauts de l’oeil. Il ne s'agit pas de connaître par coeur les causes possibles mais de savoir que des défauts peuvent exister.

* Oeil myope
Un oeil myope est un oeil qui ne peut pas voir de loin. Le Punctum Remotum est ramené à une distance proche (quelque fois quelques dizaines de centimètres).

_En général, la myopie est due à une cavité oculaire plus grande que la normale (myopie axiale) mais il arrive qu'elle soit liée à une augmentation  de l'indice de réfraction du cristallin (myopie d'indice)._

* Oeil hypermétrope
Un oeil hypermétrope au repos à tendance à faire converger les rayons derrière la rétine. Cela est souvent dû à une cavité oculaire trop petite.

_La conséquence est que l’oeil n'est jamais au repos puisqu'il doit sans cesse accommoder pour voir l'objet visé, même à l'infini. Cela entraîne souvent une fatigue oculaire plus fréquente._

* Presbytie
La presbytie, en général liée à l'âge, est la difficulté de voir de près. En général, cela est lié à une fatigue musculaire empêchant de bomber le cristallin suffisamment.

* Astigmatie
L'astigmatie est un défaut dans la symétrie axiale de l'oeil qui conduit à donner d'un point objet une image sous forme de tâche. Les images peuvent alors paraître déformée ou floue et entraîne une fatigue oculaire.
````


## Les caractéristiques de l'oeil (en ligne)
Il est utile de comprendre ce que représentent physiquement ces grandeurs mais la connaissances des valeurs précises n'est pas à connaître.

````{sidebar} Pourquoi y a-t-il une profondeur de champ?
On peut se poser la question car en effet, le stigmatisme et l'aplanétisme prévoit la conjugaison d'un objet à une image et la conjugaison du plan de la rétine avec un seul plan (celui de l'objet visé).

La raison vient du fait que l'oeil n'a pas besoin de former un point sur la rétine pour voir l'objet net ! En effet, l'oeil est constitué de cellules rétiniennes qui ont une taille finie. Si la tâche (au lieu du point) formé est plus faible que la cellules rétiniennes, l'oeil verra l'objet net même s'il n'y a pas conjugaison au sens de l'optique géométrique.

Cette "imperfection" de l'oeil (elle limite la résolution) est très utile puisqu'elle permet de voir des objets nets alors qu'ils ne sont pas dans le même plan: c'est la profondeur de champ.
````
````{topic} Caractéristiques de l'oeil
* Champ angulaire de l’oeil (ou d'un instrument d'optique) : angle d'observation maximale.
    * Exemple : Le champ angulaire d'un oeil est d'environ $160^\circ$ à $180^\circ$. Il est en pratique limité d'un côté par la présence du nez.
    * Un instrument possède aussi son champ angulaire : cf. l'appareil photographique,
    * Utilisation : Etude du champ angulaire d'un instrument (lunette utilisée par l'oeil)
* Résolution angulaire : écart angulaire minimale entre deux objets peuvent être distinguer par l'oeil.
    * La résolution angulaire de l'oeil seul est de l'ordre de $3 \times 10^{-4} \rm{rad}$.
    * La résolution angulaire est due à l'existence de cellule rétinienne dont la taille est finie. Si deux objets proches forment une image sur la même cellule rétinienne, ils ne seront pas distingués.
    * Un instrument à capteur possède aussi une résolution angulaire (appareil photographique limité par la taille de ses capteurs CCD)
    * En pratique la diffraction par la pupille limite aussi la résolution angulaire.
* Profondeur de champ : Intervalle de position donnant une image considérée comme nette par l'instrument (ici l'oeil) pour une configuration (un réglage) de l'instrument (ici pour une valeur de focale du cristallin).
````

````{topic} Profondeur de champ et appareil photographique
Il y a le même phénomène dans un appareil photographique (taille des tâches formées sur la pellicule pour l'argentique ou taille des récepteurs CCD pour le numérique).

Dans ce cas là aussi, cela permet d'avoir une profondeur de champ. Ceux qui ont fait un peu de photographie pourront associer la profondeur de champ à l'ouverture (diaphragme) de l'appareil photographique. Il en est de même pour l'oeil (rôle de la pupille).
````
````{topic} Principe de construction et d'étude d'un instrument d'optique
:class: full-width
Lorsqu'un fabricant va construire un instrument d'optique, il va chercher à assurer un confort visuel. Pour celà, il va faire en sorte que l'image finale soit au Punctum Remotum pour l'utilisateur.

* Les données dites "commerciales" sont en général données en se référant à une utilisation par un oeil emmétrope.
* Le constructeur prévoit en général un réglage permettant d'adapter l'instrument à un oeil présentant un défaut (réglage de _l'oculaire_).
````


