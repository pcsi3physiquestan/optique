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

# Lois de Snell-Descartes

Les lois de Snell-Descartes permettent de traiter le cas où l'on passe brusquement d'un milieu d'indice de réfraction $n_1$ à un milieu d'indice $n_2$.

On remarquera que localement, l'approximation de l'optique géométrique n'est plus valable. Cela explique que les propriétés précédentes ne suffisent plus à étudier le comportement des rayons lumineux.

## Lois de Snell-Descartes: Enoncé


````{dropdown} Définitions préalables
On considère un rayon lumineux, appelé __rayon incident__ qui se propage dans un milieu d'indice $n_1$ et qui arrive à la frontière - le __dioptre__ avec un milieu d'indice $n_2$ différent de $n_1$.

On définit la normale au dioptre (n) au point d'incidence I où le rayon incident intersecte le dioptre et on appelle __plan d'incidence__ le plan formé par le rayon incident et la normale (n) au dioptre.
````


````{admonition} Fondamental : Lois de Snell-Descartes (Admis)
:class: important

Lorsqu'un rayon lumineux (appelé __rayon incident__) se propageant dans un milieu d'indice $n_1$ arrive sur un __dioptre__, ce rayon sépare énergétiquement en deux rayons __tous deux contenus dans le plan d'incidence__:

* l'un, appelé __rayon réfléchi__, continue à se propager dans le milieu d'indice $n_1$.
* l'autre, appelé __rayon réfracté__, se propage dans le milieu d'indice $n_2$.

On peut définir les angles __orientés__ pour chaque rayon:

* __angle incident__ $i_1$: de la normale vers le rayon incident.
* __angle réfléchi__ $r$:  de la normale vers le rayon réfléchi.
* __angle réfracté__ $i_2$:  de la normale vers le rayon réfracté.

```{figure} ./images/optique_descartes_plus_refringent.jpg
:name: descartes
:align: center
```
On a alors les relations géométriques suivantes:

\begin{align*}
r &= - i_1\\
n_1 \sin i_1 &= n_2 \sin i_2
\end{align*}
````

````{admonition} Complément - Séparation énergétique
:class: dropdown
La loi de Snell-Descartes permet d'étudier géométriquement l'existence des deux rayons. Mais il faut préciser qu'il s'opère un division de l'énergie entre deux parts (transmise et réfléchie) __qui ne sont pas forcément égales__.

Le théorie électromagnétique (HP) permet de prévoir la répartition énergétique. On retiendra simplement qu'il n'y a pas séparation en deux parts égales et que celle-ci peut varier en fonction de l'angle d'incidence (dans certaines conditions, on peut même annuler la puissance réfléchie ou la puissance transmise).
````

## Méthode: Tracé qualitatif du rayon réfracté.

Le tracé du rayon réfléchi s'obtient par simple symétrie quel que soient les valeurs des indices. Nous allons plutôt ici voir comment on peut prévoir semi-qualitativement le tracé du rayon réfracté et nous obtiendrons plus informations très importantes. Nous travaillerons dans le plan d'incidence.

__Les conclusions obtenues ici sont à connaître autant qu'à savoir retrouver.__

Il est conseillé de réfléchir aux exercices avant de regarder les réponses.


````{admonition} Exercice 
:class: attention

On considère le cas où $n_1 < n_2 $.

1. Le rayon réfracté s'éloigne-t-il ou se rapproche-t-il de la normale?
2. Justifier que l'angle réfracté ne peut prendre qu'une gamme de valeur limitée dans le plan d'incidence.
````

````{dropdown} Correction
>* Tracé qualitatif du rayon réfracté

```{figure} ./images/optique_descartes_plus_refringent.jpg
:name: plus_refringent
:align: center
```
>
>Remarquons que $\frac{\sin i_1}{\sin i_2} = \frac{n_2}{n_1} > 1$. Or sur $[-\pi;\pi/2]$, la fonction sinus est croissante donc $i_1> i_2$.
>
>Il vient qu'au passage d'un milieu moins réfringent à un milieu plus réfringent, le rayon réfracté se rapproche de la normale
>
>* Gamme d'angle.
>
>L'étude précédente montre que quand l'angle d'incidence atteint $\pi/2$ (on parle __d'incidence rasante__), l'angle réfracté est encore inférieur l'angle droit. Il apparaît que les gammes d'angles en sortie sont limitées. On atteint pas toutes les valeurs entre $-\pi/2$ et $\pi/2$.
>
>Plus précisément, les gammes valeurs atteintes sont $i_2 \in [-\arcsin\left ( \frac{n_1}{n_2}\right); \arcsin\left ( \frac{n_1}{n_2}\right)]$
````

````{admonition} Fondamental : Bilan
:class: important
On retiendra que lors du passage d'un milieu moins réfringent à un milieu plus réfringent:

* le rayon réfracté __se rapproche de la normale__ par rapport au rayon incident
* le rayon réfracté va avoir une gamme limitée de valeur. La valeur limite $i_2 =\arcsin\left ( \frac{n_1}{n_2}\right)$ est appelée __angle de réfraction limite.__
````

````{admonition} Exercice 
:class: attention

On considère le cas où $n_2 < n_1 $.

1. Le rayon réfracté s'éloigne-t-il ou se rapproche-t-il de la normale?
2. Justifier que l'angle réfracté va atteinte une réfraction rasante (égale à $\pm \pi/2$ pour un angle d'incidence strictement inférieure à $\pm \pi/2$ (en valeur absolue). On notera $i_0$ la valeur limite de l'angle d'incidence.
3. Que se passe-t-il si l'angle d'incidence est supérieure à $i_0$ ?
````

````{dropdown} Correction
>* Tracé qualitatif du rayon réfracté
>
>Remarquons que $\frac{\sin i_1}{\sin i_2} = \frac{n_2}{n_1} < 1$. Or sur $[-\pi;\pi/2]$, la fonction sinus est croissante donc $i_1 < i_2$.
>
>Il vient qu'au passage d'un milieu moins réfringent à un milieu plus réfringent, le rayon réfracté s'éloigne de la normale
>
>* Gamme d'angle.
>
>L'étude précédente montre que quand l'angle de réfraction atteint $\pm \pi/2$, l'angle d'incidence est encore inférieur l'angle droit. L'angle limite d'incidence est $i_0 = \pm \arcsin\left ( \frac{n_2}{n_1}\right)$.
>
>* Réflexion totale.
>
>Si l'angle d'incidence est supérieure à $i_0$, on observe expérimentalement qu'il n'y a pas de rayon réfracté. On parle de __réflexion totale__: toute la lumière est réfléchie.
````

````{admonition} Fondamental : Bilan
:class: important
On retiendra que lors du passage d'un milieu plus réfringent à un milieu moins réfringent:

* le rayon réfracté __s'éloigne de la normale__ par rapport au rayon incident
* si l'angle d'incidence devient trop grand, il y a phénomène de __réflexion totale__, c'est-à-dire que toute la lumière est réfléchie.

L'angle d'incidence limite permettant la réfraction se calcule en cherchant un angle réfracté de $\pm \pi/2$. On obtient: 

\begin{equation}
i_0 = \pm \arcsin\left ( \frac{n_2}{n_1}\right)
\end{equation}
````

````{dropdown} Remarque : Angle de réfraction limite.
Dans le cas où $n_1 > n_2$, on devrait parler pour désigner $i_0$ d'angle d'incidence limite (sous-entendu permettant la réfraction).	

Ce n'est pas le cas. On l'appelle...  __angle de réfraction limite__.

...  C'est un peu dérangeant car il s'agit bien de la valeur de l'angle d'incidence et non de l'angle de réfraction... 

Pourquoi cette confusion ? A cause du principe de retour inverse. En effet, on pourra remarquer que les deux $i_0$ introduit dans les deux exercices sont identiques en inversant les indices $n_1$ et $n_2$, soit en réalisant une propagation de la lumière...  en sens inverse !

Et le principe de retour inverse nous indique que si du milieu d'indice $n_1$ vers le milieu d'indice $n_2$ un angle d'incidence $i_0$ donne un angle de réfraction $\pi/2$, alors en passant du milieu d'indice $n_2$ vers le milieu d'indice $n_1$ avec un angle d'incidence de $\pi/2$, l'angle de réfraction sera de $i_0$: c'est bien le même angle !

Si l'abus de langage est à connaître surtout pour ne pas se tromper face à un énoncé, la réflexion sur le principe de retour inverse et son utilisation est fondamental. __Essayez de bien le comprendre et même de faire un dessin pour visualiser ce principe.__
````

## Utilisation des lois de Snell-Descartes

````{admonition} Exercice 
:class: attention

```{figure} ./images/exo_casserole.png
:name: casserole
:align: center
:width: 40%
```

On considère une pièce de monnaie de rayon $R_0$ dont on négligera l'épaisseur posée au fond d'une casserole de hauteur $H_0$ remplie à ras bord d'eau.

L'oeil d'un observateur se trouve à la verticale de centre de la pièce à une hauteur $H_1$.

1. On appelle O le centre de la pièce. Déterminer l'équation que vérifie l'ouverture angulaire $\theta_0$ du faisceau issu du point O et qui entre dans l’oeil en fonction du rayon de la pupille $R_1$.

2. **Faire l'application numérique pour $H_0 = H_1$ en choisissant  des valeurs numériques plausibles. On sera amener à simplifier l'équation précédente AVANT de la résoudre en justifiant les simplification réalisée par des ordres de grandeurs.
````

````{dropdown} Correction
>1. __Mise en équation__
>
>Notons le point I, le point d'incidence sur le dioptre air-eau pour le rayon extrême du faisceau issu de O et entrant dans la pupille. On note $i_1$ et $i_2$ les angles respectivement d'incidence et de réfraction. On a les relations :
>
>\begin{align*}
	n_{eau} \sin i_1 &= n_{air} \sin i_2\\
	\frac{IL}{\tan i_2} &= H_1\\
	IL + IJ &= R_1\\
	\tan i_1 &= \frac{IJ}{H_0}
\end{align*}
>
>On a 4 inconnues (IL, IJ, $i_1$ et $i_2$) et quatre inconnues, on peut donc résoudre le système.
>
>Il est important de voir que la résolution complète ne nous intéresse pas. On veut $i_1$ qui représente l'ouverture angulaire. On va donc chercher à __garder ____$i_1$____ et éliminer les autres inconnues.__
>
>Les grandeurs $H_0, H_1, R_1$ et les indices sont des grandeurs connues qu'on va garder.
>
>__Equation pour l'angle__
>Les deux dernières équations permettent d'écrire: $IJ = H_0 \tan i_1$ et $ IL = R_1 - H_0 \tan i_1$ d'où le système:
>
>\begin{align*}
	n_{eau} \sin i_1 &= n_{air} \sin i_2\\
	\frac{R_1}{\tan i_2} - H_0 \frac{\tan i_1}{\tan i_2}&= H_1
\end{align*}
>soit en éliminant $i_2$ (on a directement utilisant $n_{air} = 1$ -  on peut se le permettre car l'indice de réfraction est sans dimension: le changer par sa valeur numérique n'impacte pas l'analyse dimensionnelle):
>
>\begin{equation}
\left ( R_1 - H_0 \tan i_1 \right )\sqrt{1 - n_{eau}^2 \sin^2 i_1} = H_1 n_{eau} \sin i_1
\end{equation}
>
>On rappelle que $\theta_0 = i_1$

2. Résolution aux petits angles

Nous allons faire une approximation pour résoudre cette équation (sans quoi la résolution devient TRÈS délicate). En effet, la taille de la pupille est de l'ordre du mm (on prendra $R_1 = 1\rm{mm}$) et la hauteur de la casserole est de l'ordre de la dizaine de cm. (on prendre $R_0 = 5\rm{cm}$). Il vient que les angles à la normale seront nécessairement petit.

On peut avoir un ordre de grandeur en considérant que $\theta_0 \sim \arctan\frac{R_0}{2H_0} \sim 10^{-2} \rm{rad}$. En pratique, la propagation n'est pas rectiligne mais les angles $i_1$ et $i_2$ sont nécessairement du même ordre de grandeur que $\theta_0$.

Or si $\theta_0 << 1$, on __peut faire les approximations dites des petits angles :__

\begin{align*}
	\sin i &\approx i\\
	\tan i &\approx i\\
	\cos i &\approx 1\\
\end{align*}

On ne conservera pas aussi les puissances au carré des petits angles (on parle d'approximation à l'ordre 1), des précisions seront données sur cette approximation dans des cours ultérieurs. On essaiera déjà d'appréhender la méthode d'utilisation de cette approximation.

Ici l'équation devient :

\begin{equation}
\left ( R_1 - H_0 i_1 \right ) = H_1 n_{eau} i_1 \Longrightarrow \theta_0 = i_1 \approx \frac{R_1}{H_0 + H_1} = 10^{-2}  \rm{rad}
\end{equation}
````
