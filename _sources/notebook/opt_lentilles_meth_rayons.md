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

# Méthodes : Tracés graphiques
## Tracé un rayon transmis quelconque.
Les corrections sont en ligne. __Il est important de s'entraîner à rédiger la descrpition du tracé.__
_Vous pouvez visualiser la méthode de tracé d'une image grâce à [cette simulation Geogebra](https://stanislas.edunao.com/mod/resource/view.php?id=12786)._

````{admonition} Exercice 
:class: attention

On considère un rayon arrivant sur la lentille ci-dessous. Représenter le rayon transmis.

```{figure} ./images/lentille_cv_rayon.png
:name: l_rayon_exo
:align: center
:width: 50%
```
````

````{topic} Méthode
> Le principe de construction est le suivant: deux rayons incidents parallèles ressortent en se croisant dans le plan focal image. On va donc:
> 
> 1. tracer un rayon utile parallèle au rayon qui nous intéresse. Ici, on a tracé (pointillés rouges) le rayon passant par le centre optique qui ressort non dévié).
> 2. chercher sont intersection avec le plan focal image (point D)
> 3. le rayon sortant qui nous intéresse passant par D, il ne reste plus qu'à le tracer.
> 
```{figure} ./images/lentille_cv_rayon_2.png
:name: l_rayon_corr
:align: center
:width: 50%
```
````

## Déterminer un point image.

````{admonition} Exercice 
:class: attention

On considère un point B hors de l'axe optique. Déterminer graphiquement son image B' par la lentille ci-dessous.

```{figure} ./images/lentille_cv_obj_ha.png
:name: l_objet_exo
:align: center
:width: 50%
```
````

````{topic} Méthode
>Puisqu'on est dans les conditions de Gauss, on considère le stigmatisme réalisé. On va donc tracer deux rayons et chercher l'intersection des deux rayons transmis. Ce sera l'image B'. On a le choix entre les trois rayons utiles.
>
>Ici, __on a tracé les 3 mais deux suffisent__, on a représenté les 3 à titre d'entraînement.
>
```{figure} ./images/lentille_cv_obj_ha_2.png
:name: l_objet_corr
:align: center
:width: 50%
```
````

````{admonition} Exercice 
:class: attention

On considère un point A sur l'axe optique. Déterminer graphiquement son image A' par la lentille ci-dessous.

```{figure} ./images/lentille_cv_obj_sa.png
:name: l_objet_a_exo
:align: center
:width: 50%
```
````

````{topic} Méthode
>Cette fois, on ne peut tracer directement deux rayons utiles (les 3 sont le même: l'axe optique). Par contre, on peut utiliser l'aplanétisme: un point hors de l'axe optique (B) mais dans le plan frontal de A aura une image B' dans le même plan frontal que A'.
>
>Une fois B placé, on cherche son image comme précédemment et on la projette sur l'axe optique pour obtenir A'.
>
>Ici, __on a tracé les 3 mais deux suffisent__, on a représenté les 3 à titre d'entraînement.
>
```{figure} ./images/lentille_cv_obj_sa_2.png
:name: l_objet_a_corr
:align: center
:width: 50%
```
````

## Tracé un faisceau transmis

````{admonition} Exercice 
:class: attention

On considère le faisceau suivant arrivant sur une lentille convergente. Tracer le faisceau sortant correspondant.

```{figure} ./images/lentille_cv_faisceau.png
:name: l_cv_faisceau
:align: center
:width: 50%
```
````

````{topic} Méthode
>Il existe deux méthodes pour obtenir le tracé du faisceau sortant: on passe par un point objet ou l'on trace les rayons sortants extrêmes.
>
>__Méthode 1.__ : Le principe est le suivant: le faisceau entrant concourent en un point (ici C). Le faisceau sortant va donc concourir en un point C' qui sera l'image de C par la lentille. On va chercher la position de C' puis on tracera les rayons extrêmes (qui passent par C' donc) pour obtenir le faisceau sortant.
>
>On a réalisé la construction ci-dessous en utilisant deux rayons: l'un passant par C et le centre optique, l'autre par C et le foyer principal objet. Le faisceau sortant est hachuré vert.
>
```{figure} ./images/lentille_cv_faisceau_2.png
:name: l_cv_faisceau_corr
:align: center
:width: 50%
```
>
>__Méthode 2.__ : On utilise cette fois les méthodes vues pour tracer le devenir d'un rayon quelconque. On a, sur la figure ci-dessous, tracé deux rayons: chacun est parallèle à un rayon extrême et passe par le centre optique. On cherche leurs intersections avec le plan focal image: les deux rayons extrêmes doivent passer par ces intersections. On a donc le faisceau sortant.
>
```{figure} ./images/lentille_cv_faisceau_3.png
:name: l_cv_faisceau_corr_2
:align: center
:width: 50%
```
````
