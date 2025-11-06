---
mainfont: Alegreya
title: Gérer des collections d'images avec XnView et Tropy
date: 1^er^ semestre 2025-2026
author: sebastien.biay@univ-nantes.fr
lang: fr-FR
---

Gérer des collections d'images avec XnView et Tropy
=====

Plan :

1. [Classement (archivage) et information](#t1)
	1. [Reproductions d'œuvres ](#t1-1)
	2. [Reproductions d'ouvrages ](#t1-2)
2. [Traiter des fichiers-images par lots](#t2)

<!--FINET-->


<a id='t1'/>

# Classement (archivage) et information
[comment1]: <1> (TITRE1)

<a id='t1-1'/>

## Reproductions d'œuvres 

### <2>


![](/home/sbiay/nextcloud/enseignement/cours/NUM1/daumier/collections/france/paris-orsay/crispin-scapin-RF-2057/orsay-1.jpg)


- Créer un dossier `daumier` sur un disque externe (ou sur le PC)
- Accéder à [cette notice](https://www.musee-orsay.fr/fr/oeuvres/crispin-et-scapin-10867)
- Télécharger l'image
- L'archiver dans une arborescence de dossiers incluse dans le dossier `daumier`


### <3>

On associe de l'information à l'image de trois manières :

1. **Chemin** de l'image (arbre des dossiers qui la contiennent)

2. **Nom** de l'image

3. **Métadonnées** de l'image :\
	L'image téléchargée en contient-elle ?\
	De quel type ?

4. Joindre un fichier texte


### <4>


![](/home/sbiay/nextcloud/enseignement/cours/NUM1/daumier/collections/france/paris-louvre/amateurs-estampes-RF-4036/768.jpg)


- Accéder à [cette notice](https://arts-graphiques.louvre.fr/detail/oeuvres/1/16708-Les-amateurs-destampes-max)
- Télécharger l'image
- Consulter les métadonnées


### <5>

**Renseigner les métadonnées de la reproduction de *Crispin et Scapin*** :

- Cliquer sur l'œuvre
- Ctrl + I pour afficher la boîte de dialogue des métadonnées IPTC[^400]
- Se concentrer sur le volet **Crédit**

[^400]: Modèle standard développé par l'International Press Telecommunications Council.


### <6>

Les droits de reproduction détenus par la RMN coûtent cher…

- Télécharger [cette image](https://commons.wikimedia.org/wiki/File:Honor%C3%A9_daumier,_crispino_e_scapino,_1864_ca._02.JPG) utilisable gratuitement
- Renseigner les métadonnées de Crédit
- Insérer le type de licence dans le champ **Crédits**
	
	- Le plus efficace est de faire un clic droit sur `Attribution 3.0 Unported`
	- Copier l'hyperlien
	- Le coller dans Crédit > **Crédits**

<a id='t1-2'/>

## Reproductions d'ouvrages 

### <7>


- Télécharger depuis Madoc le dossier compressé **cat-exp-1999.zip**

- Comment nommer le dossier où archiver cet ouvrage de manière à :
	- Respecter les conventions de nommages (pas d'espace, etc.) ?
	- Faire facilement le lien entre Zotero et le dossier ?

- **Une solution** : télécharger l'extension [BetterBibTex](https://retorque.re/zotero-better-bibtex/)\
	pour Zotero [ici](https://github.com/retorquere/zotero-better-bibtex/releases/latest)

### <8>

- Créer un dossier `loyretteDaumier18081879Cat1999` dans l'arborescence `daumier` et y dézipper les fichiers
- Ouvrir le dossier dans XnView


<a id='t2'/>

# Traiter des fichiers-images par lots
[comment4]: <8> (TITRE1)


### <9>

- Sélectionner toutes les images sauf la première

	- Crtl + A
	- Ctrl + clic gauche sur la première

- Édition > Renommer (F2)

- La dernière et l'avant-dernière image sont dans l'ordre inversé (cela peut toujours arriver !)

	- Cliquer sur la dernière image
	- La faire remonter d'un cran à l'aide des boutons à flèches de droite

- Donner comme nouveau nom `p-###` :
	- début `352`,
	- pas `2`  le pas est le rythme d'implémentation de la numérotation d'item en item

- **Ok**

On obtient une numérotation continue des fichiers par numéros de pages

### <10>

On peut enrichir des noms de fichiers en conservant les noms actuels

Ajoutons le titre de cette partie du catalogue : "Théâtre, Molière"

- Sélectionner à nouveau les fichiers
- Cliquer sur la flèche de droite à côté du champ **Modèle de nom**
- Choisir **Nom de fichier**
- A la suite, écrire : `-theatre-moliere`
- Ok


### <11>

Il faudrait améliorer le contraste de ces photos, et comme la couleur ne sert à rien, les passer en niveaux de gris donnerait des fichiers plus légers…

1. Sélectionner toutes les images

2. Cliquer droit sur une image > Conversion par lots

3. Actions 

	- Ajouter action > Image > Modifier le nombre de couleurs > **Niveaux de gris**

	- Ajouter action > Table > Niveaux : modifier la Luminosité

5. Sortie
	
	- Créer un **Dossier**: `photos-livre-modif`

	- **Convertir**


### <12>

Faire des photos avec son téléphone, c'est rapide ; récupérer des clichés en HD des œuvres que l'on étudie, c'est encore mieux.


**Image** : [Sacramentaire de Gellone, fol. 18r](img/lat-12048-sacramentaire-gellone_fol-018r-detail-a.jpg)

1. Accéder à [**cette page**](https://gallica.bnf.fr/ark:/12148/btv1b60000317/f43) sur Gallica

2. La télécharger en JPG et l'afficher dans XnView  


### <13>


**Image** : [Sacramentaire de Gellone, fol. 18r](img/lat-12048-sacramentaire-gellone_fol-018r-detail-a.jpg)

Remarquer le logo\
[](/home/sbiay/ater/M1NUM/demos/logo-iiif.png)
dans la partie gauche de l'interface de Gallica.

IIIF = *International Image Interoperability Framework*, une communauté d'institutions patrimoniales qui proposent un cadre d'**interopérabilité** (qui fonctionne de la même manière dans toutes les institutions) pour partager des images en HD sur le web.

Ce partage se fait via une **API** (*Application Programming Interface*), une interface web uniquement pour les programmeurs et les machines, et non pas un site web que l'on peut visiter.


### <14>


**Image** : [Sacramentaire de Gellone, fol. 18r](img/lat-12048-sacramentaire-gellone_fol-018r-detail-a.jpg)

Pour accéder à l'image depuis l'API Gallica modifier l'URL comme ceci : 

gallica.bnf.fr/

**iiif**/

ark:/12148/btv1b60000317/f43/

**full/full/0/native.jpg**

*****

Télécharger l'image au même endroit que la première fois, comparer les métadonnées des images.\
Qu'en déduisez-vous ?


### <15>

L'API permet de modifier le fichier image en intervenant sur les paramètres de son URL. Cliquer sur les points suivants et regarder en quoi l'URL est différente :

1. [Rotation à 90°](https://gallica.bnf.fr/iiif/ark:/12148/btv1b60000317/f43/full/full/90/native.jpg)

2. [Résolution limitée à 1200 px de largeur](https://gallica.bnf.fr/iiif/ark:/12148/btv1b60000317/f43/full/1200,/0/native.jpg)

2. [Résolution limitée à 1200 px de hauteur](https://gallica.bnf.fr/iiif/ark:/12148/btv1b60000317/f43/full/,1200/0/native.jpg)


### <16>

1. Copier l'URL https://gallica.bnf.fr/ark:/12148/btv1b60000317/f43 et la coller dans [**Dezoomify**](https://dezoomify.ophir.dev/)

2. Télécharger cette nouvelle image et la comparer aux autres, notamment la métadonnée « Dimension »

>

Remarque, l'image téléchargée de Dezoomify est plus lourde (PNG 34 bits au lieu de Jpeg 24 bits).\
Pour la transformer en Jpeg plus léger dans XnView : Faire un clic droit sur l'image > Convertir en > JPG


### <17>

Dezoomify est capable d'extraire des photos en HD depuis des collections en ligne :

- Où le téléchargement en définition moyenne, comme l'**Art Institute de Chicago** (voir la chambre de Van Gogh [**ici**](https://www.artic.edu/artworks/28560/the-bedroom))

- Où le téléchargement n'est pas proposé ! comme la **British Library** (voir le Psautier Vespasien [**ici**](https://www.bl.uk/manuscripts/Viewer.aspx?ref=cotton_ms_vespasian_a_i_f030v))

Vous pouvez coller les URL de ces pages dans Dezoomify et accéder au fichier.

**NB** : trouver l'URL d'une image est parfois tout un jeu de piste…


### <18>

Des extensions de navigateur pour aller plus vite :

1. Dezoomify est aussi une extension de Firefox [**ici**](https://addons.mozilla.org/fr/firefox/addon/dezoomify/)

2. [**Geobib**](http://www.geobib.fr/tool/iiif/) peut télécharger des images HD de **Gallica** en un clic


### <19>

1. Manuscrits et livres rares : voir la plateforme [**Biblissima**](https://iiif.biblissima.fr/collections/)

2. Inventaires des collections par l'[**Université de Leyde**](https://www.library.universiteitleiden.nl/binaries/content/assets/ul2ub/bijzondere-collecties/list-of-iiif-collections.pdf)


### <20>

1. Le fichier contenant toutes les URL des images s'intitule comme ceci : [https://gallica.bnf.fr/iiif/ark:/12148/btv1b60000317/manifest.json](https://gallica.bnf.fr/iiif/ark:/12148/btv1b60000317/manifest.json)

2. Pour trouver les URL des images, ouvrir ce fichier dans Firefox

3. Parcourir l'arborescence : sequences > *numéro* > canvases > *numéro* > images > *numéro* > resource > **\@id**

4. Si \@id ne se termine pas par `.jpg`, essayer d'ajouter `/full/full/0/default.jpg` ou `/full/full/0/native.jpg`


