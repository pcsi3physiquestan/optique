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
# Entrainement : Lentilles minces
_Ces exercices seront traités en classe, individuellement ou en groupe._

## Etude graphique d'une lentille divergente
On considère une lentille divergente. Déterminer les images (il est conseillé de refaire des dessins à chaque fois pour des questions de clarté):


````{admonition} Exercice 
:class: attention

1. du rayon entrant __j__
2. de l'objet AB
3. de l'objet CD

```{figure} ./images/ex_td_dv_graphique_1.png
:name: ex_td_dv_g_1
:align: center
```
````

On considère une lentille divergente. Déterminer les antécédents (il est conseillé de refaire des dessins à chaque fois pour des questions de clarté):


````{admonition} Exercice 
:class: attention
1. du rayon sortant __j'__
2. de l'image A'B'
3. de l'image C'D'

```{figure} ./images/ex_td_dv_graphique_2.png
:name: ex_td_dv_g_2
:align: center
```
````

_Point utile pour cet exercice_
* _$\Longrightarrow$ [Méthode : Tracés graphiques](traces_gr)._

## Etude d'un doublet
On considère un doublet de lentille, c'est-à-dire deux lentilles $L_1$ et $L_2$ de distance focale image respectives $f_1  = a$ et $f_2 = 3a$ et dont les centre optique (respectivement $O_1$ et $O_2$) sont distants de $\overline{O_1 O_2} = 2a$.


````{admonition} Exercice 
:class: attention
1. Déterminer graphiquement la position du foyer objet.
2. Déterminer graphiquement la position du foyer image.
3. Déterminer par le calcul la position du foyer objet. _Pensez à vérifier la cohérence de vos résultats._
4. Déterminer par le calcul la position du foyer image. _Pensez à vérifier la cohérence de vos résultats._
````

````{topic} Eléments de réponse (sans justification)
1. $\overline{F_1 A} = \frac{a}{2}$
2. $\overline{F'_2 A'} = - \frac{9a}{2}$
````

_Point utile pour cet exercice_
* _$\Longrightarrow$ [Méthode : Tracés graphiques](traces_gr)._
* _$\Longrightarrow$ [Méthode : Etude qualitative](lentille_qu)._
* _$\Longrightarrow$ [Relations de conjugaison](conjugaison)._
* _$\Longrightarrow$ [Eléments principaux d'un système centré](foyers)._


## L'oeil et ses défauts
On désire étudier l'oeil et l'un de ses défauts: la myopie. On modélise l'oeil par une lentille convergente représentant le cristallin (distance focale image $f'$, centre optique O) qui doit former l'image de l'objet observé sur la rétine qu'on modélisera par un écran situé en $A'$ à une distance $e=\overline{OA'}=15\rm{mm}$. L'oeil observe un objet situé en A à une distance $\overline{AO}=d$.


````{admonition} Exercice 
:class: attention

* Rappeler la définition du Punctum Proximum (noté ici $P_P$) et du Punctum Remotum (noté ici $P_R$). On note $d_m=\overline{P_P O}$ et $D_m=\overline{P_R O}$ leur position respective (en valeur absolue) sur l'axe optique de l'oeil. Donner leur valeur pour un oeil normal (dit emmétrope), on note la valeur de $d_m$ pour l'oeil emmétrope $d_{m0}$.
* On note $V$ la vergence d'un cristallin pour un oeil emmétrope. $V$ est une fonction de $d$. Déterminer $V(d)$. Montrer que la vergence augmente quand l'objet est de plus en plus proche.
* Déterminer $V(D_{m0})$ et $V(d_{m0})$. L'oeil est au repos quand il observe un objet dans le plan du Punctum Remotum, la valeur $V(D_{m0})$ est donc la vergence du cristallin quand l'oeil est au repos.
````

On suppose un oeil myope où le cristallin est trop convergent (cas de myopie assez rares). On note sa vergence $V_m$. Celle-ci peut varier entre deux valeurs extrêmes qui sont: $V(d_{m0})+\delta V$ et $V(D_{m0})+\delta V$ avec $\delta V > 0$ et constant quelque soit la position d de l'objet observé. On appelle $\delta_V$ le degré de myopie.


````{admonition} Exercice 
:class: attention
* Un oeil myope et un oeil emmétrope observent tous deux un objet situé à une distance d (pour les deux yeux) de sorte que les deux yeux voient l'objet net. Quelle est la différence de vergence entre les deux cristallin?
* Déterminer en fonction de $d_{m0}$ et $\delta V$, la position du $P_P$ (notée $d_{mm}$) et du $P_R$ (notée $D_{mm}$) pour un oeil myope. Justifier qu'on dise que le degré de myopie est l'inverse de la distance du Punctum Remotum.
* Calculer leur position pour $\delta V=0.1\delta; \delta V=4\delta; \delta V=10\delta$. Commenter.
* On désire corriger un oeil myope grâce à une lentille de contact qu'on accole au cristallin (en première approximation). Quel est le type de lentille qu'on doit choisir et quelle est sa vergence?
````

On désire corriger un oeil myope grâce à un verre de lunette qu'on considère être une lentille de vergence $V'$ dont le centre optique O' est situé à $d_L=\overline{O'O}=2\rm{cm}$


````{admonition} Exercice 
:class: attention
* Déterminer la valeur de $V'$ en fonction de $\delta V$ et $d_L$ pour que l'oeil myope puisse alors observer un objet à l'infini net tout en étant au repos. A.N. $\delta V=4\delta$
* Par abus de langage, on appelle degré de myopie la vergence du verre correcteur (en valeur absolue) qu'il faut mettre devant un oeil pour corriger sa myopie. A quelle condition sur $\delta V$ et $d_L$, cette abus est-il acceptable?
* Dans le cas où $\delta V=4\delta$, calculer la nouvelle position du $P_P$, on notera cette distance (dans le sens positif) $d_{mc}$. Que devient cette distance dans le cas où $\delta V \ll 1/d_L$?
````
_Point utile pour cet exercice_
* _$\Longrightarrow$ [Méthode : Etude qualitative](lentille_qu)._
* _$\Longrightarrow$ [Relations de conjugaison](conjugaison)._
* _$\Longrightarrow$ [L'oeil : Accomodation]((oeil_acco))._
* _$\Longrightarrow$ [Lentilles accolées](lentilles_acco)._