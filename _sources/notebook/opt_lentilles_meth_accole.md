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

# Activités : Lentilles accolées

Nous allons étudier ici le cas de deux lentilles minces accolées, __c'est-à-dire de deux lentilles dont on peut considerer que les centres optiques sont confondus.__

````{admonition} Exercice 
:class: attention
Montrer que __deux lentilles accolées de vergence $V_1$ et $V_2$ sont équivalentes à une seule lentille dont le centre optique est placé au même endroit que ceux des lentilles accolées et dont la vergence est $V = V_1 + V_2$
````

````{topic} Correction
Soit un objet $A$ dont l'image par $L_1$ (image intermédiaire) et appelé $A_1$. On appelle $A_2$ l'image de $A_1$ par $L_2$ (image finale). $A$ est supposé sur l'axe optique. On note $O$ le centre optique __commun_ aux deux lentilles par hypothèse. On a donc le schéma de transformation:

$$
A \overbrace{\longrightarrow}^{L_1(O,f'_1)} A_1 \overbrace{\longrightarrow}^{L_2(O,f'_2)} A_2
$$

On peut donc écrire les deux relations de conjugaison:
\begin{equation}
\begin{cases}
\frac{1}{\overline{OA_1}} - \frac{1}{\overline{OA}} &= V_1\\
\frac{1}{\overline{OA_2}} - \frac{1}{\overline{OA_1}} &= V_2
\end{cases}
\end{equation}
soit en sommant les deux relations:

$$
\frac{1}{\overline{OA_2}} - \frac{1}{\overline{OA}} = V_1 + V_2
$$

_Tout se passe donc bien comme s'il n'y avait qu'une seule lentille conjuguant $A$ et $A_2$ de vergence $V_1 + V_2$ et située en $O$._
````
````{important} Bilan à retenir - Ce n'est PAS la correction
On retiendra:
* la conclusion de l'exercice
* __que cette conclusion n'est pas QUE si les lentilles sont accolées__.
````
