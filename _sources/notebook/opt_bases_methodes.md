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

# Activité

## Tracé qualitatif du rayon réfracté.
Le tracé du rayon réfléchi s'obtient par simple symétrie quel que soient les valeurs des indices. Nous allons plutôt ici voir comment on peut prévoir semi-qualitativement le tracé du rayon réfracté et nous obtiendrons plus informations très importantes. Nous travaillerons dans le plan d'incidence.

_Vous pouvez utiliser la [simulation Geogebra en ligne](https://moodlecpge.stanislas.fr/mod/resource/view.php?id=111) pour visualiser les différents comportements._
__Les conclusions obtenues ici sont à connaître autant qu'à savoir retrouver.__

Il est __vivement__ conseillé de réfléchir aux exercices __avant__ de regarder les réponses (en ligne).


````{admonition} Exercice 
:class: attention

On considère le cas où $n_1 < n_2 $.

1. Le rayon réfracté s'éloigne-t-il ou se rapproche-t-il de la normale?
2. Justifier que l'angle réfracté ne peut prendre qu'une gamme de valeur limitée dans le plan d'incidence.
````

````{topic} Correction
>__Tracé qualitatif du rayon réfracté__

```{figure} ./images/optique_descartes_plus_refringent.jpg
:name: plus_refringent
:align: center
```
>
>Remarquons que $\frac{\sin i_1}{\sin i_2} = \frac{n_2}{n_1} > 1$. Or sur $[-\pi;\pi/2]$, la fonction sinus est croissante donc $i_1> i_2$.
>
>Il vient qu'au passage d'un milieu moins réfringent à un milieu plus réfringent, le rayon réfracté se rapproche de la normale.
>
>__Gamme d'angle__
>
>L'étude précédente montre que quand l'angle d'incidence atteint $\pi/2$ (on parle __d'incidence rasante__), l'angle réfracté est encore inférieur l'angle droit. Il apparaît que les gammes d'angles en sortie sont limitées. On atteint pas toutes les valeurs entre $-\pi/2$ et $\pi/2$.
>
>Plus précisément, les gammes valeurs atteintes sont $i_2 \in [-\arcsin\left ( \frac{n_1}{n_2}\right); \arcsin\left ( \frac{n_1}{n_2}\right)]$
````

````{important} __Bilan - A retenir__
:class: full-width
On retiendra que lors du passage d'un milieu moins réfringent à un milieu plus réfringent:

* le rayon réfracté __se rapproche de la normale__ par rapport au rayon incident
* le rayon réfracté va avoir une gamme limitée de valeur. La valeur limite $i_2 =\arcsin\left ( \frac{n_1}{n_2}\right)$ est appelée __angle de réfraction limite.__
````

````{admonition} Exercice 
:class: attention

On considère le cas où $n_2 < n_1 $.

1. Le rayon réfracté s'éloigne-t-il ou se rapproche-t-il de la normale?
2. Justifier que l'angle réfracté va atteinte une réfraction rasante (égale à $\pm \pi/2$ pour un angle d'incidence strictement inférieure à $\pm \pi/2$. On notera $i_0$ la valeur limite de l'angle d'incidence.
3. Que se passe-t-il si l'angle d'incidence est supérieure à $i_0$ ?
````

````{topic} Correction
>__Tracé qualitatif du rayon réfracté__
>
>Remarquons que $\frac{\sin i_1}{\sin i_2} = \frac{n_2}{n_1} < 1$. Or sur $[-\pi;\pi/2]$, la fonction sinus est croissante donc $i_1 < i_2$.
>
>Il vient qu'au passage d'un milieu moins réfringent à un milieu plus réfringent, le rayon réfracté s'éloigne de la normale
>
>__Gamme d'angle__
>
>L'étude précédente montre que quand l'angle de réfraction atteint $\pm \pi/2$, l'angle d'incidence est encore inférieur l'angle droit. L'angle limite d'incidence est $i_0 = \pm \arcsin\left ( \frac{n_2}{n_1}\right)$.
>
>__Réflexion totale__
>
>Si l'angle d'incidence est supérieure à $i_0$, on observe expérimentalement qu'il n'y a pas de rayon réfracté. On parle de __réflexion totale__: toute la lumière est réfléchie.
````

(snell_totale)=
````{important} __Bilan - A retenir__
:class: full-width
On retiendra que lors du passage d'un milieu plus réfringent à un milieu moins réfringent:

* le rayon réfracté __s'éloigne de la normale__ par rapport au rayon incident
* si l'angle d'incidence devient trop grand, il y a phénomène de __réflexion totale__, c'est-à-dire que toute la lumière est réfléchie.

L'angle d'incidence limite permettant la réfraction se calcule en cherchant un angle réfracté de $\pm \pi/2$. On obtient: 

$$
i_0 = \pm \arcsin\left ( \frac{n_2}{n_1}\right)
$$
````

````{sidebar} Angle de réfraction limite.
Dans le cas où $n_1 > n_2$, on devrait parler pour désigner $i_0$ d'angle d'incidence limite (sous-entendu permettant la réfraction).	

Ce n'est pas le cas. On l'appelle...  __angle de réfraction limite__.

...  C'est un peu dérangeant car il s'agit bien de la valeur de l'angle d'incidence et non de l'angle de réfraction... 

Pourquoi cette confusion ? A cause du __principe de retour inverse__. En effet, on pourra remarquer que les deux $i_0$ introduit dans les deux exercices sont identiques en inversant les indices $n_1$ et $n_2$, soit en réalisant une propagation de la lumière...  en sens inverse !

Et le principe de retour inverse nous indique que si du milieu d'indice $n_1$ vers le milieu d'indice $n_2$ un angle d'incidence $i_0$ donne un angle de réfraction $\pi/2$, alors en passant du milieu d'indice $n_2$ vers le milieu d'indice $n_1$ avec un angle d'incidence de $\pi/2$, l'angle de réfraction sera de $i_0$: c'est bien le même angle !

Si l'abus de langage est à connaître surtout pour ne pas se tromper face à un énoncé, la réflexion sur le principe de retour inverse et son utilisation est fondamental. __Essayez de bien le comprendre et même de faire un dessin pour visualiser ce principe.__
````