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

# TD : Bases de l'optique

_Ces exercices seront traités en classe._

## Fibre optique à saut d'indice

__Objectifs:__ Établir les expressions du cône d'acceptance et de la dispersion intermodale d'une fibre à saut d'indice.

Une fibre optique à saut d'indice est constituée d'un coeur en silice d'indice $n_1$ entouré d'une gaine d'indice $n_2$. Le tout est à symétrie cylindrique. Elle permet de transporter des informations par modulation d'amplitude d'un faisceau lumineux confiné à l'intérieur de la fibre par réflexion totale.

```{figure} ./images/fibre_optique.jpg
:name: fibre
:align: center
Fibre optique
```

La perte en transmission (ou atténuation) $X$ s'exprime par $X_{dB}=10\log(\frac{P_2}{P_1})$ avec $P_1$ la puissance lumineuse à l'entrée de la fibre et $P_2$ la puissance lumineuse au bout d'un kilomètre dans la fibre. On l'exprime en $\rm{dB.km^{-1}}$ 


````{admonition} Exercice 
:class: attention

1. Quelle condition doit-on imposer à $n_2$ et $n_1$ pour pouvoir confiner la lumière dans la fibre (c'est-à-dire pour qu'il y ait réflexion totale) ?
2. Sachant qu'en 1970, l'atténuation était de $-10\rm{dB.km^{-1}}$ et qu'actuellement elle est de $-0.005\rm{dB.km^{-1}}$, déterminer dans les deux cas les pertes en puissance en \% au bout d'un km.
3. Un rayon lumineux arrive en I avec un angle $\theta_i$. Montrer que si $\theta_i$ est inférieur à un angle $\theta_a$, un rayon peut être guidé à travers le coeur. Pour une fibre cylindrique, justifier le terme de __cône d'acceptance.__
4. On appelle ouverture numérique (O.N.) la grandeur $\sin(\theta_a)$. Donner l'expression de O.N. en fonction de $n_1$ et de $\Delta=\frac{n_1^2-n_2^2}{2n_1^2}$. A.N.: $\Delta=10^{-2},n_1=1,5$.

Une impulsion lumineuse (une information) arrive à t = 0 au point O sous la forme d'un faisceau conique de demi-angle au sommet (O) $\theta_i$ ($\theta_i<\theta_a$).

5. Pour une fibre de longueur l, calculer l'élargissement temporel (ou __dispersion intermodale__) $\Delta t$ à la sortie de la fibre, c'est-à-dire le temps écoulé entre la sortie du premier rayon et celle du dernier. On l'exprimera en fonction de $l, n_1, c$ et $\theta_i$.
6. En déduire quelle quantité d'information cette fibre peut transmettre en une seconde. A.N.: $l=10km,\theta_i=8^{\circ},n_1=1,5$
````

````{topic} Eléments de réponse (sans justification)
* $n_2 < n_1$
* 90\% puis 0.1\%
* $\theta_a = \arcsin{\sqrt{n_1^2 - n_2^2}}$
* $sin \theta_a = n_1 \sqrt{2 \Delta} = 0.2$
* $\Delta t = \frac{n_1 l}{c} \left( \frac{1}{\sqrt{1 - {\left(\frac{\sin \theta_i}{n_1}\right)}}^2} - 1 \right)$
* $\Delta t = 50 \rm{\mu s} $
````

## TD: Arc-en-ciel
On désire étudier le phénomène de l'arc-en-ciel au moyen d'un modèle simple. On suppose ici que les gouttes d'eau sont assimilables à des sphères de rayon R, de centre O et d'indice de réfraction homogène n = 1,3 baignant dans l'air.

La sphère est éclairée par un faisceau de lumière parallèle, dont un rayon atteint la sphère en A. Après réfraction, le rayon retouche le dioptre eau-air en B. Le rayon alors réfléchi recoupe la sphère en C où un rayon refracté ressort avec une angle $\widehat{a}$ par rapport à l'axe Ox. On pose $\widehat{i}$ l'angle incident au point A et $\widehat{r}$ l'angle réfracté au même point A (c'est-à-dire l'angle $\widehat{OAB}$). On supposera que $\widehat{a} \in [0;\pi/2 ]$.

```{figure} ./images/arc_en_ciel.jpg
:name: label_image
:align: center
Arc-en-ciel
```

````{admonition} Exercice 
:class: attention
1. Pourquoi suppose-t-on que le faisceau incident est un faisceau de rayons parallèles ? Quelle est sa direction ?
2. Quelles sont alors les valeurs possibles de l'angle $\widehat{i}$ ?
3. Peut-il y avoir réflexion totale en B?
4. Montrer que $\widehat{a}=4\widehat{r}-2\widehat{i}$.
5. En déduire $\widehat{a}$ en fonction de $\widehat{i}$ seulement.
6. Calculer $\frac{d\widehat{a}}{d\widehat{i}}$
7. Montrer qu'il existe un angle $i_{\max}$ pour lequel $\widehat{a}$ est maximal. Calculer $i_{\max}$ et $a_{\max}$.
8. Montrer que si un observateur regarde haut dans le ciel avec un angle $\widehat{a}$ qu'on précisera, il recevra un maximum de lumière (il y aura accumulation des rayons lumineux).
````
````{topic} Eléments de réponse (sans justification)
1. ...
2. $[-\pi/2;\pi/2]$
3. Non
4. ... 
5. $a = 4 \arcsin\frac{\sin i}{n} - 2 i$
6. $\frac{\rm{d}a}{\rm{di}} = 4 \frac{\frac{\cos i}{n}}{\sqrt{1 - \frac{\sin^2 i}{n^2}}} - 2$
7. $i_{\max} = \arccos\sqrt{ \frac{n^2-1}{3}} = 1.07 \rm{rad}$ et $a_{\max} = 0.82 \rm{rad}$

Cet observateur ne verra alors les gouttes "briller" que sur un cône d'axe de révolution (observateur-direction des rayons provenant du soleil) et de demi-angle au sommet (qui est l'observateur) $a_{\max}$. Généralement l'horizon empêche d'observer complètement le cône.
````

````{admonition} Exercice 
:class: attention
8. Dans des conditions telles que le soleil soit à l'ouest, incliné de $10^{\circ}$ au-dessus de l'horizon. De quel côté faut-il regarder pour observer un arc-en-ciel? Préciser la hauteur angulaire maximale $\alpha$ au-dessus de l'horizon et les circonstances météorologiques nécessaires à l'observation.

On explique le phénomène de l'arc-en-ciel par les propriétés dispersives de l'eau, c'est-à-dire que l'indice de réfraction de l'eau varie en fonction de la longueur d'onde de la lumière.

9. Déterminer les valeurs maximum de a pour le rouge (n=1,331) et pour le violet (n=1,337) et en déduire quelle couleur fera l'extérieur de l'arc-en-ciel (c'est-à-dire la partie la plus haute). Que vaut l'ouverture angulaire $\Delta\alpha$ de l'arc-en-ciel?
````

````{topic} Eléments de réponse (sans justification)
Soleil dans le dos, sous un angle $a_{\max} - \alpha$
````

## La déviation par le prisme
Il s'agit d'une activité d'approfondissement permettant d'essayer de s'entraîner sur un exercice plus difficile. Certains points pourront être utiles plus tard en Travaux Pratiques.

Principe général: On considère un prisme triangulaire d'angle au sommet A dont la base est posée horizontalement sur un socle. On envoie un faisceau lumineux constitué de rayon parallèle sur une des face et on observe les rayons sortant par l'autre face (les deux faces constituant l'angle A). Ce seront les deux faces utiles du prisme. Le faisceau étant parallèle l'angle que font les rayons avec la première face du prisme est toujours la même, on note cet angle i. Il vient par les lois de Descartes que les angles formées par les différents rayons réfractés seront les mêmes quelques soit le rayon considéré. On va donc considéré un seul rayon pour l'étude.

But: On désire étudier la déviation du rayon lumineux D en fonction de l'angle d'incidence i. L'air extérieur est considéré comme un milieu d'indice 1.

```{figure} ./images/optique_prisme_deviation.jpg
:name: prisme
:align: center
Déviation par le prisme
```

````{admonition} Exercice 
:class: attention
1. Etablir une relation entre i,r et n puis entre i', r' et n.
2. Montrer que $A=r+r'$ et $D=i+i'-A$.
3. Existence d'un rayon dévié.
    1. \*Quelles sont les valeurs de i telles qu'on observe effectivement un rayon sortant du prisme? On ne tiendra pas compte des limitations géométriques du prisme. Déterminer cette gamme pour $n=1,5$ et $A=60^{\circ}$. On notera $i_0$, l'angle limite qui apparaî dans le raisonnement.
    2. Que se passe-t-il si l'angle du prisme est trop grand ($90^{\circ}$ par exemple)?
    3. Faire un tracé des rayons et déterminer l'angle de déviation D pour les cas $i=i_0$ et $i=\pi/2$. Commenter.
4. Déduire de la question précédente que la fonction $D(i)$ passe par au moins un extremum. L'expérience montre qu'il y en a qu'un seul et que c'est un minimum de déviation. On notera $D_m$ le minimum de déviation.
5. \*Retrouver le résultat de l'expérience par une étude mathématique de la fonction $D(i)$.
6. Quelle est la relation entre $D_m$, A et n?
7. En général, le prisme choisi est très dispersif c'est-à-dire que l'indice de réfraction n dépend fortement (tout est relatif) de la longueur d'onde du faisceau incident $\lambda$. Expliquer pourquoi un tel dispositif permet la réaliser d'un spectroscope, c'est-à-dire un appareil permettant de déterminer le spectre d'un signal lumineux.
8. (Recherche) Expliquez comment Newton a utiliser cette méthode pour montrer que la lumière blanche était composé d'un grand nombre de radiations "élémentaires". Commenter ce terme (et précisez le terme utilisé aujourd'hui).
````
