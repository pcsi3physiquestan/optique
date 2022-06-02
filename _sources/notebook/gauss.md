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

# Stigmatisme approché et condition de Gauss

Comme nous l'avons précisé précédemment, seul le miroir plan permet de réaliser un stigmatisme rigoureux. Mais on utilise pourtant des miroirs sphériques, des lentilles...  Et l'on arrive à voir des images nettes.

Pour ce faire, on doit se placer dans un cadre moins "rigoureux" mais suffisant à cause des "imperfections" de notre oeil: le __stigmatisme approché__.

## Stigmatisme approché

### Absence de stigmatisme rigoureux (en ligne)

````{topic} Absence de stigmatisme: Cas du dioptre plan
On observe sur la simulation suivante où le faisceau issu du point $A_1$ ressort sans converger en un point précis. Il n'y a donc pas stigmatisme rigoureux.

Nous verrons sur des simulations ultérieures que le miroir sphérique ne réalise pas non plus de stigmatisme rigoureux.

```{figure} ./images/optique_dioptre_aberration.jpg
:name: plan_aberration
:align: center
:width: 50%
```
````

````{topic} Se rapproché du stigmatisme
Si l'on ne peut réaliser un stigmatisme rigoureux, on peut essayer s'en rapprocher en __sélectionnant__ certains rayons qui passent tous à peu près en un même point.

On peut le voir sur le cas du dioptre sur le schéma suivant. On a uniquement gardé les rayons peu inclinés et on peut considérer en première approximation qu'ils convergent en un point. Plus précisément en une tâche suffisamment petite pour que notre oeil ne puisse la distinguer d'un point.

```{figure} ./images/optique_dioptre_diaphragme.jpg
:name: plan_diaphragme
:align: center
:width: 50%
```

C'est en sélectionnant les rayons qu'on pourra s'approcher du stigmatisme et donc réaliser...  __un stigmatisme approché__.
````


### Stigmatisme approché: sélection des rayons

````{important} __Stigmatisme approché__
:class: full-width
On dit qu'un système réalise un stigmatisme approché pour un couple de points (A;A') si tous les rayons lumineux du faisceau issu du point A _et traversant le système optique_ ressortent __au voisinage__ du point A'.

A' sera considéré comme l'image de l'objet A par le système optique et on dira que A' et A sont conjugués.
````

## Conditions de Gauss

### Condition de Gauss: Simulation

On utilisera ici un miroir sphérique pour réaliser la simulation du tracé des rayons. On utilise un point objet à l'infini dans un premier temps puis une simulation sur un objet à distance finie sera produite.


````{panels}
```{figure} ./images/optique_spherique_proche_axe.jpg
:name: spherique_axe
:align: center
Objet à l'infini sur l'axe optique (__pas A__). Sélection des rayons proches.
```
---
```{figure} ./images/optique_spherique_peu_incline.jpg
:name: spherique_incline
:align: center
Objet à l'infini hors de l'axe optique (__pas A__). Sélection des rayons peu inclinés ET proches.
```

---
```{figure} ./images/optique_spherique_objet_fini.jpg
:name: spherique_fini
:align: center
Objet à distance finie (point A). Sélection des rayons peu inclinés ET proches.
```
````

### Condition de Gauss: Présentation

````{important} __Conditions de Gauss__
:class: full-width
Les conditions de Gauss (ou condition des rayons paraxiaux) sont un cadre théorique et expérimental dans lequel on sélectionne uniquement les rayons sont satisfont aux deux conditions:

* ils ne doivent pas être trop inclinés par rapport à l'axe optique.
* ils doivent entrer dans le système optique en un point proche de l'axe optique.

__Un système centré placé dans les conditions de Gauss réalise un stigmatisme approché.__
````

```{margin}
Si cette propriété est hors programme, on verra qu'elle sera nécessaire pour expliquer la méthode de recherche d'image par les lentilles.
```
````{topic} Complément : Aplanétisme (HP)
Il n'est pas nécessaire de le retenir mais se placer dans les conditions de Gauss permet aussi de réaliser un aplanétisme approché.
````

### Conditions de Gauss: Réalisation expérimentale

En pratique, on va réaliser les conditions de Gauss en:
* mettant un diaphragme en amont du système optique pour empêcher les rayons trop éloignés d'entrer.
* mettant un diaphragme en aval du système optique (ou à l'intérieur) pour couper le passage des rayons trop inclinés.

### Condition de Gauss: Utilisation analytique

```{margin}
Attention pour les applications numériques, les valeurs des angles __doivent être en radians__.
```
````{important} __Approximations aux petits angles__
Dans le cadre des conditions de Gauss, il vient que les angles avec l'axe optique sont petits. On utilisera alors l'approximation des petites angles sur les fonctions trigonométriques:
\begin{align*}
	\sin i &\approx i\\
	\tan i &\approx i\\
	\cos i &\approx 1 \text{ ou } 1 - \frac{i^2}{2} \textrm{ (si l'on a besoin de plus de précision.)}\\
\end{align*}
````

### Condition de Gauss: Aberrations

Si les conditions de Gauss ne sont pas respectées expérimentalement, cela donne lieu à des __aberrations géométriques__, c'est-à-dire que l'image sera déformée ou floue.

```{figure} ./images/abb_coussinet.jpg
:name: abberation
:align: center
```

