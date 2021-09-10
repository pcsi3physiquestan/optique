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

# Activité méthode : Les bases

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

1. Quelle condition doit-on imposer à $n_2$ et $n_1$ pour pouvoir confiner la lumière dans la fibre (c'est-à-dire pour qu'il y ait réflexion totale)?
2. Sachant qu'en 1970, l'atténuation était de $-10\rm{dB.km^{-1}}$ et qu'actuellement elle est de $-0.005\rm{dB.km^{-1}}$, déterminer dans les deux cas les pertes en puissance en \% au bout d'un km.
3. Un rayon lumineux arrive en I avec un angle $\theta_i$. Montrer que si $\theta_i$ est inférieur à un angle $\theta_a$, un rayon peut être guidé à travers le coeur. Pour une fibre cylindrique, justifier le terme de __cône d'acceptance.__
4. On appelle ouverture numérique (O.N.) la grandeur $\sin(\theta_a)$. Donner l'expression de O.N. en fonction de $n_1$ et de $\Delta=\frac{n_1^2-n_2^2}{2n_1^2}$. A.N.: $\Delta=10^{-2},n_1=1,5$.

Une impulsion lumineuse (une information) arrive à t = 0 au point O sous la forme d'un faisceau conique de demi-angle au sommet (O) $\theta_i$ ($\theta_i<\theta_a$).

5. Pour une fibre de longueur l, calculer l'élargissement temporel (ou __dispersion intermodale__) $\Delta t$ à la sortie de la fibre, c'est-à-dire le temps écoulé entre la sortie du premier rayon et celle du dernier. On l'exprimera en fonction de $l, n_1, c$ et $\theta_i$.
6. En déduire quelle quantité d'information cette fibre peut transmettre en une seconde. A.N.: $l=10km,\theta_i=8^{\circ},n_1=1,5$
````

````{dropdown} Eléments de réponse (sans justification)
* $n_2 < n_1$
* 90\% puis 0.1\%
* $\theta_a = \arcsin{\sqrt{n_1^2 - n_2^2}}$
* $sin \theta_a = n_1 \sqrt{2 \Delta} = 0.2$
* $\Delta t = \frac{n_1 l}{c} \left ( \frac{1}{\sqrt{1 - {\left(\frac{\sin \theta_i}{n_1}}\right)}^2} - 1\right)$
* $\Delta t = 50 \rm{\mu s} $
````