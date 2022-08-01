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
# Exemple d'étude: la loupe

## La loupe: Principe
Une loupe sert à grossir les objets. Elles composée d'une lentille (convergente).

Les caractéristiques intéressantes de la loupe sont:
* son grossissement - plus précisément son grossissement commercial.
* sa latitude de mise au point: on recherchera l'intervalle de position d'objet pouvant être vue par l'oeil - on placera l'oeil au foyer image de la loupe de façon arbitraire.
* sa profondeur de champ et sa résolution angulaire (pour un oeil emmétrope). Nous ne calculerons ici que la résolution angulaire.

## Caractéristiques d'une loupe
Vous pouvez essayer de faire l'exercice au moyen des définitions précédentes.

````{admonition} Exercice 
:class: attention
On considère une loupe constituée d'une lentille convergente de distance focale image$f'$. Pour les applications numériques, on prendra $f' = 10 mm$

1. Déterminer l'intervalle de position de l'objet permettant à un oeil emmétrope (on donne la distance du PR: $d_{min} = 25 \rm{mm}$) de voir l'image donnée par la loupe nette. On supposera que l'oeil est placé au foyer image de la loupe et que $d_{min} > f'$.
2. Déterminer le grossissement commercial de la loupe.
3. Déterminer la taille du plus petit objet distinguable par l'oeil dans les conditions d'utilisation optimales. On donne le pouvoir de résolution de l'oeil: $\theta = 3 \times 10^{-4} \rm{rad}$
````

````{dropdown} Correction
__Q1. Latitude de mise au point__

On va chercher les antécédents du PR et du PP. L'intervalle entre les deux correspondra à la latitude de mise au point.

L'antécédent du Punctum Remotum - qui est à l'infini - est évidemment le foyer principal objet de la loupe donc $\overline{FA_{PR}} = 0$

On cherche l'antécédent du Punctum Proximum positionné tel que $\overline{F'A'_{PP}} = - d_{min}$.

Puisque qu'on a déjà la distance au foyer image, on va utiliser la relation de Newton:

$$
\overline{FA_{PP}} \times \underbrace{\overline{FA'_{PP}}}{-d_{\min}} = - f'^2 \Longrightarrow \boxed{\overline{FA_{PP}} = \frac{f'^2}{d_{\min}}}
$$
Application numérique: la largeur de l'intervalle est 4mm.

__Q2. Grossissement commercial__

__Calcul de l'angle apparent à travers la loupe.__ L'image finale devant être au PR d'un oeil emmétrope, donc à l'infini, son antécédent doit être au foyer principal objet.

On considère un objet $\overline{AB}$ placé dans le plan focal objet. On a représenté le tracé pour obtenir l'image B' de B par la loupe. On peut ainsi déterminer l'angle sous lequel on voit l'image à travers la loupe.

```{figure} ./images/loupe_grossissement.png
:name: loupe_gr
:align: center
:width: 60%
```

Il vient $\alpha' \approx \tan \alpha ' = -\frac{\overline{AB}}{f'}$

__Calcul de l'angle à l'oeil nu__. Il vient directement $\alpha \approx \tan \alpha = -\frac{\overline{AB}}{d_{\min}}$

On obtient le grossissement:

$$
G_c = \left\vert \frac{\alpha'}{\alpha} \right\vert = \frac{d_{\min}}{f'}
$$

Application numérique: $G_c = \times 25$

__Q3. Plus petit objet distinguable.__
On peut reprendre les formules précédentes:

$$
AB = f' \tan \theta \approx \theta f' \approx 3 \times 10^{-6} \rm{rad}
$$
````

````{dropdown} Remarque
__Analyse de la latitude de mise au point et du grossissement.__

On remarque que la latitude de mise au point diminue très rapidement avec la distance focale.

A l'inverse, le grossissement augmente quand la distance focale diminue. On a donc un compromis entre le grossissement et la latitude de mise au point: plus on augmente le premier, plus la seconde est délicate.

Diminuer la distance focale peut avoir d'autres limites, notamment l'obligation de bomber la lentille ce qui conduit à des aberrations plus importantes.
````