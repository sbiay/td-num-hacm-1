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

1. [Classement et information](#t1)
	1. [Classement et information](#t1-1)
	2. [Classement et information](#t1-2)
	3. [Classement et information](#t1-3)
	4. [Classement et information](#t1-4)
	5. [Classement et information](#t1-5)
	6. [Classement et information](#t1-6)
	7. [Classement et information](#t1-7)
2. [Traiter des fichiers-images par lots](#t2)
	1. [Renommer les fichiers](#t2-1)
	2. [Renommer les fichiers](#t2-2)
	3. [Modifier des images par lots](#t2-3)
3. [Récupérer des images en HD](#t3)
	1. [Récupérer des images en HD depuis Gallica](#t3-1)
	2. [Récupérer des images en HD depuis Gallica](#t3-2)
	3. [Modifier les paramètres de l'adresse](#t3-3)
	4. [Modifier les paramètres de l'adresse](#t3-4)
	5. [Pour récupérer plus facilement des images en HD](#t3-5)
	6. [Pour récupérer plus facilement des images en HD](#t3-6)
	7. [Des collections accessibles au format iiif](#t3-7)
	8. [Pour les *geeks* : fouiller un *manifest*](#t3-8)
4. [Organiser une collection d'images avec Tropy](#t4)
	1. [Démarrer](#t4-1)
	2. [Démarrer un projet](#t4-2)
	3. [Démarrer un projet](#t4-3)
	4. [Démarrer un projet](#t4-4)
	5. [Métadonnées DC](#t4-5)
	6. [Métadonnées DC : créateur](#t4-6)
	7. [Métadonnées DC : créateur](#t4-7)
	8. [Métadonnées DC : titre, etc.](#t4-8)
	9. [Métadonnées DC : type](#t4-9)
	10. [Métadonnées DC : type](#t4-10)
	11. [Métadonnées DC : source](#t4-11)
	12. [Métadonnées DC : identificateur](#t4-12)
	13. [Métadonnées DC : format](#t4-13)
	14. [Métadonnées DC : format](#t4-14)
	15. [Métadonnées DC : sujet, couverture](#t4-15)
	16. [Métadonnées DC : autres](#t4-16)
	17. [Indexer une lithographie parue dans la presse](#t4-17)
	18. [Indexer une lithographie parue dans la presse](#t4-18)
	19. [Indexer un document d'archive](#t4-19)
	20. [Transcrire un document en note](#t4-20)
	21. [Grouper les objets par listes](#t4-21)
	22. [Fermer et rouvrir le projet](#t4-22)

<!--FINET-->



<a id='t1'/>

# Classement et information
[comment1]: <1> (TITRE1)


<a id='t1-1'/>

## Classement et information

On associe de l'information à l'image de trois manières :

1. **Chemin** de l'image (arbre des dossiers qui la contiennent)

2. **Nom** de l'image

3. **Métadonnées** de l'image :\
	L'image téléchargée en contient-elle ?\
	De quel type ?

4. Joindre un fichier texte


<a id='t1-2'/>

## Classement et information


![](/home/sbiay/nextcloud/enseignement/cours/NUM1/daumier/collections/france/paris-orsay/crispin-scapin-RF-2057/orsay-1.jpg)


- Créer un dossier `daumier` sur le PC (on n'aura pas besoin de conserver son contenu passée la séance)
- Accéder à [\textcolor{bluecette notice}](https://www.musee-orsay.fr/fr/oeuvres/crispin-et-scapin-10867)
- Télécharger l'image
- L'archiver dans une arborescence de dossiers incluse dans le dossier `daumier`


<a id='t1-3'/>

## Classement et information


![](/home/sbiay/nextcloud/enseignement/cours/NUM1/daumier/collections/france/paris-louvre/amateurs-estampes-RF-4036/768.jpg)


- Accéder à [\textcolor{bluecette notice}](https://arts-graphiques.louvre.fr/detail/oeuvres/1/16708-Les-amateurs-destampes-max)
- Télécharger l'image
- Consulter les métadonnées grâce au logiciel **XnView MP**, préinstallé sur les PC de la salle ou téléchargeable [\textcolor{blueici}](https://www.xnview.com/fr/xnview/)


<a id='t1-4'/>

## Classement et information

**Renseigner les métadonnées de la reproduction de *Crispin et Scapin*** :

- Cliquer sur l'œuvre
- **Ctrl + I** pour afficher la boîte de dialogue des métadonnées IPTC[^400]
- Se concentrer sur le volet **Crédit**

[^400]: Modèle standard développé par l'International Press Telecommunications Council.


<a id='t1-5'/>

## Classement et information

Les droits de reproduction détenus par la RMN coûtent cher…

- Télécharger [\textcolor{bluecette image}](https://commons.wikimedia.org/wiki/File:Honor%C3%A9_daumier,_crispino_e_scapino,_1864_ca._02.JPG) utilisable gratuitement
- Renseigner les métadonnées de Crédit
- Insérer le type de licence dans le champ **Crédits**
	
	- Le plus efficace est de faire un clic droit sur `Attribution 3.0 Unported`
	- Copier l'hyperlien
	- Le coller dans Crédit > **Crédits**


<a id='t1-6'/>

## Classement et information

- Télécharger depuis Madoc le dossier compressé **cat-exp-1999.zip**

- Comment nommer le dossier où archiver cet ouvrage de manière à :
	- Respecter les conventions de nommages (pas d'espace, etc.) ?
	- Faire facilement le lien entre Zotero et le dossier ?

- **Une solution** de nommage pour les reproductions de réf. bibliographiques : l'extension [\textcolor{blueBetterBibTex}](https://retorque.re/zotero-better-bibtex/) pour Zotero\
	à télécharger [\textcolor{blueici}](https://github.com/retorquere/zotero-better-bibtex/releases/latest)

	- Cliquer droit sur le fichier **.xpi** pour l'enregistrer sous
	- Dans Zotero : **Outils** > Extensions
	- Cliquer sur la **roue dentée** > Install plugin from file


<a id='t1-7'/>

## Classement et information

Chaque référence Zotero possède désormais une **clé de citation** en tête de notice, idéale pour nommer des fichiers ou des dossiers en lien avec la référence :

- Créer un dossier `loyretteDaumier18081879Cat1999` dans l'arborescence `daumier` et y dézipper les fichiers
- Ouvrir le dossier dans XnView


<a id='t2'/>

# Traiter des fichiers-images par lots
[comment2]: <8> (TITRE1)


<a id='t2-1'/>

## Renommer les fichiers

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

-  **Ok**

On obtient une numérotation continue des fichiers par numéros de pages

<a id='t2-2'/>

## Renommer les fichiers

On peut enrichir des noms de fichiers en conservant les noms existant

Ajoutons le titre de cette partie du catalogue :\
« Théâtre, Molière » après la numérotation des pages :

- Sélectionner à nouveau les fichiers
- Cliquer sur la flèche de droite,\
	à côté du champ **Modèle de nom**
- Choisir **Nom de fichier**
- A la suite, écrire : `-theatre-moliere`
- Ok


<a id='t2-3'/>

## Modifier des images par lots

Si l'on souhaite modifier les couleurs ou le contraste des images :

1. Sélectionner toutes les images

2. Cliquer droit sur une image > **Conversion par lots**

3. Actions 

	- Ajouter action > Image > Modifier le nombre de couleurs > **Niveaux de gris**

	- Ajouter action > Table > Niveaux : modifier la Luminosité

5. Sortie
	
	- Nom de fichier : `NB-Filename`

	- **Convertir**


<a id='t3'/>

# Récupérer des images en HD
[comment3]: <11> (TITRE1)

<a id='t3-1'/>

## Récupérer des images en HD depuis Gallica
[comment4]: <12> (TITRE2)


**Image** : [*La promenade du critique influent, estampe*, BnF](img/charivari-1865-06-24_btv1b525144764_f1.jpg)


1. Accéder à [\textcolor{bluecette page}](https://gallica.bnf.fr/ark:/12148/btv1b525144764/f1) sur Gallica

2. La télécharger en JPG et l'afficher dans XnView  


<a id='t3-2'/>

## Récupérer des images en HD depuis Gallica


Remarquer le logo dans la partie gauche de l'interface de Gallica.

![](/home/sbiay/illustrations-cours/cours/NUM1/logos/iiif_logo.jpg)
*International Image Interoperability Framework*, une communauté d'institutions patrimoniales qui proposent un cadre d'**interopérabilité** (qui fonctionne de la même manière dans toutes les institutions) pour partager des images en HD sur le web.

Ce partage se fait via une **API** (*Application Programming Interface*), une interface web uniquement pour les programmeurs et les machines.

URL de consultation Gallica :\
`https://gallica.bnf.fr/ark:/12148/btv1b525144764/f1`

URL de l'image sur l'API IIIF en résolution maximale :\

`https://gallica.bnf.fr/iiif/ark:/12148/btv1b525144764/f1/full/full/0/native.jpg`


<a id='t3-3'/>

## Modifier les paramètres de l'adresse

L'API permet de modifier le fichier image en intervenant sur les paramètres de son URL.

https://gallica.bnf.fr/iiif/ark:/12148/btv1b525144764/f1/ \
\textcolorbluefull/\textcolororangefull/\textcolorpurple{0}/native.jpg

Cliquer sur les points suivants et regarder en quoi l'URL est différente :


1. [\textcolor{blueZone d'intérêt dans l'image}](https://gallica.bnf.fr/iiif/ark:/12148/btv1b525144764/f1/954,3172,1432,1198/full/0/native.jpg)

2. \textcolororangeRésolution :

	1. [\textcolor{grayRésolution limitée à 1200 px de largeur}](https://gallica.bnf.fr/iiif/ark:/12148/btv1b525144764/f1/full/1200,/0/native.jpg)

	2. [\textcolor{grayRésolution limitée à 1200 px de hauteur}](https://gallica.bnf.fr/iiif/ark:/12148/btv1b525144764/f1/full/,1200/0/native.jpg)

3. [\textcolor{purpleRotation à 90°}](https://gallica.bnf.fr/iiif/ark:/12148/btv1b525144764/f1/full/full/90/native.jpg)


<a id='t3-4'/>

## Modifier les paramètres de l'adresse

![](/home/sbiay/illustrations-cours/NUM1/images/zone-interet.jpg)
**Zone d'intérêt**


Ordre des paramètres :    \textcolorred{3}  \textcolorolive{4}    \textcolorblue{1} \textcolororange{2}


URL : …/f1/**\textcolorred954,\textcolorolive3172,\textcolorblue1432,\textcolororange1198**/full/0/native.jpg


<a id='t3-5'/>

## Pour récupérer plus facilement des images en HD

Un autre moyen d'accéder à la HD de certaines images zoomables :

1. Copier l'URL `https://gallica.bnf.fr/ark:/12148/btv1b525144764/f1` et la coller dans [\textcolor{blueDezoomify}](https://dezoomify.ophir.dev/)

2. Télécharger cette nouvelle image et, dans XnView, la comparer à la précédente, en consultant la métadonnée « Dimension »

Remarque, l'image téléchargée de Dezoomify est plus lourde (PNG 34 bits au lieu de Jpeg 24 bits).\
Pour la transformer en Jpeg plus léger dans XnView : Faire un clic droit sur l'image > Convertir en > JPG


<a id='t3-6'/>

## Pour récupérer plus facilement des images en HD


Des extensions de navigateur pour aller plus vite :

1. Dezoomify est aussi une extension de Firefox [\textcolor{blueici}](https://addons.mozilla.org/fr/firefox/addon/dezoomify/) :

	- Installer l'extension
	- Se placer sur une page avec une image zoomable
	- Cliquer sur le bouton de l'extension pour l'activer
	- Zoomer sur l'image
	- Si l'extension change d'aspect, recliquer dessus…

2. [\textcolor{blueGeobib}](http://www.geobib.fr/tool/iiif/) peut télécharger des images HD et en Jpeg de **Gallica** en un clic


<!--
<a id='t3-7'/>

## Des collections accessibles au format iiif

Des sites publics d'archives
https://archives.valdoise.fr/ark:/18127/1030621.1415874/dao/0

1. Manuscrits et livres rares : voir la plateforme [\textcolor{blue**Biblissima**}](https://iiif.biblissima.fr/collections/)

2. Inventaires des collections par l'[\textcolor{blue**Université de Leyde**}](https://www.library.universiteitleiden.nl/binaries/content/assets/ul2ub/bijzondere-collecties/list-of-iiif-collections.pdf)


<a id='t3-8'/>

## Pour les *geeks* : fouiller un *manifest*

1. Le fichier contenant toutes les URL des images s'intitule comme ceci : [\textcolor{bluehttps://gallica.bnf.fr/iiif/ark:/12148/btv1b60000317/manifest.json}](https://gallica.bnf.fr/iiif/ark:/12148/btv1b60000317/manifest.json)

2. Pour trouver les URL des images, ouvrir ce fichier dans Firefox

3. Parcourir l'arborescence : sequences > *numéro* > canvases > *numéro* > images > *numéro* > resource > **\@id**

4. Si \@id ne se termine pas par `.jpg`, essayer d'ajouter `/full/full/0/default.jpg` ou `/full/full/0/native.jpg`

-->

<a id='t4'/>

# \LARGE Organiser  une collection d'images avec Tropy
[comment5]: <19> (TITRE1)


<a id='t4-1'/>

## Démarrer
[comment6]: <20> (TITRE2)

[comment7]: <20> (Logiciel développé par le Roy Rosenzweig Center for History and New Media de l'Université George Mason adapté à la gestion du vrac de photos que l'on fait lors de ses consultations mutiples[^401].)

[comment8]: <20> ([^401]: @leePersonalImageManagement2021.)


Télécharger et installer [\textcolor{blueTropy}](https://tropy.org/)

Principes et limites :\

- Il ne stocke pas d'image

- Il ajoute aux images stockées sur l'ordinateur des couches d'informations :

	- Filtres (position, luminosité, etc.) qui n'affectent pas les fichiers sources
	- Métadonnées descriptives
	- Listes
	- *Tags*, étiquettes

- Gère les fichiers images, les PDF
- Ne gère pas les fichiers audio ou vidéo


Par conséquent, il permet de structurer et de re-structurer une collection d'images au fil de sa constitution sans affecter les fichiers archivés.

[comment9]: <20> (À un stade exploratoire, pour annoter des collections et des objets. Ne permet pas de formaliser un corpus, mais de créer des listes d'objets ou des listes de collections par intérêt. Grande **malléabilité** du mode de classement : faire et défaire des listes est simple, on agrège aisément des objets.)


<a id='t4-2'/>

## Démarrer un projet

- Lancer le programme
- Nommer le projet `daumier`
- L'enregistrer sous

Interface similaire à Zotero, mais logiciel conçu pour créer des **objets** (par exemple, une œuvre d'art, une archive, etc.) que l'on décrit au moyen d'un **modèle de saisie**.

- Accéder par le menu à **Edition** > Préférences
- Le logiciel en propose plusieurs pour les **objets** :\

	- Tropy Generic
	- Dublin Core
	- Tropy Correspondence

- Choisir par défaut **Dublin Core**\
	
	très utilisé pour les données patrimoniales pour son interopérabilité : voir le descriptif de la BNF [\textcolor{blueici}](https://www.bnf.fr/fr/dublin-core)

<a id='t4-3'/>

## Démarrer un projet

On peut aussi créer son propre modèle et ainsi personnaliser le catalogage de ses objets :

- **Préférences** > Modèles de saisie
- Donner un nom
- **Créer**
- Les propriétés proposées sont très nombreuses…

La création d'un modèle personnel suppose de bien connaître et comprendre les modèles de données existant (skos, foaf, rdfs) et les propriétés qu'ils proposent\
C'est plutôt réservé aux experts en ingénierie documentaire


<a id='t4-4'/>

## Démarrer un projet

- Récupérer l'archive **daumier.zip**
- L'extraire (sur le Bureau ou dans le dossier Documents)
- Naviguer jusqu'au sous-dossier `paris-orsay\crispin-scapin-RF-2057`
- Faire glisser les deux images dans Tropy
- Puis, dans Tropy, faire glisser une image sur l'autre pour les regrouper en un seul **Objet**
- Naviguer jusqu'au dossier `paris-louvre\amateurs-estampes-RF-4036` pour créer un second objet

<a id='t4-5'/>

## Métadonnées DC
[comment10]: <24> (TITRE2)


**Mission**\
Renseigner les métadonnées [\textcolor{blueDublin Core}](https://www.bnf.fr/fr/dublin-core) pour les objets créés :

- En respectant la définition de chaque propriété DC
- En utilisant des vocabulaires contrôlés


<a id='t4-6'/>

## Métadonnées DC : créateur

- **Créateur** :
	
	- Chercher l'artiste dans le répertoire [\textcolor{blueULAN}](https://www.getty.edu/research/tools/vocabularies/ulan/)
	- Entrer dans la notice
	- Copier la forme d'autorité du nom, inscrite en début de page, juste sous **Page link**, avec les parenthèses
	- Sélectionner un seul objet dans Tropy pour l'instant
	- Coller
	- Modifier ensuite le créateur pour ne conserver entre parenthèses que les dates

<a id='t4-7'/>

## Métadonnées DC : créateur

Pour appliquer le même créateur au second objet :

- Méthode 1 : utiliser l'autocomplétion des champs
- Méthode 2 :
	- Sélectionner les deux objets
	- Ouvrir le champ Créateur
	- Appuyer sur Entrée


<a id='t4-8'/>

## Métadonnées DC : titre, etc.


![](/home/sbiay/nextcloud/enseignement/cours/NUM1/daumier/collections/france/paris-orsay/crispin-scapin-RF-2057/orsay-1.jpg)


-  Accéder à [\textcolor{bluela notice}](https://www.musee-orsay.fr/fr/oeuvres/crispin-et-scapin-10867)
- Renseigner les champs les plus intuitifs :
	- Titre
	- Date : pour conserver des dates triables, rejeter la partie texte entre parenthèses : `1864 (vers)`


<a id='t4-9'/>

## Métadonnées DC : type

**Type** définit la nature ou le genre du contenu, Dublin Core recquiert l'un des douze types suivants :\

-  collection
- dataset
- event
- image
- interactive resource
- moving image
- physical object
- service
- software
- sound
- still image <= *pour une œuvre d'art de type peinture*
- text


Mais on va privilégier un thésaurus francophone plus spécifique aux œuvres d'art…

<a id='t4-10'/>

## Métadonnées DC : type


Parmi les thésaurus de l'INHA (liste complète [\textcolor{blueici}](https://thesaurus.inha.fr/thesaurus/page/vocabulaires)) :

- Accéder au thésaurus **Type d'œuvre** [\textcolor{bluelà}](https://thesaurus.inha.fr/thesaurus/page/ark:/54721/8e09cc44-abef-4f14-9761-6c9cb3f63b2d) et trouver le descripteur le plus adapté et le plus précis (en cliquant sur les termes pour descendre dans la hiérarchie)

- Copier la donnée dans le champ **Type**

- Conserver ouvert ce thésaurus de l'INHA ou le sauvegarder dans des **Marque-pages** (Ctrl + D dans Firefox)


<a id='t4-11'/>

## Métadonnées DC : source

La définition du champ **source** est difficile à comprendre : *« référence à une ressource dont la ressource décrite est dérivée »*.\
En clair, c'est là que l'on renseigne la **cote** du document de manière complète, en incluant le **lieu de conservation**

On utilise un **référentiel d'autorité** pour saisir le nom de l'institution (cela peut éviter de commettre des approximations typographiques) :

- Chercher le musée d'Orsay sur [\textcolor{blueData-BNF}](https://data.bnf.fr/fr)
- On saisit l'information en rétablissant la ville (que Data-BNF rejette après un point) en première position, suivie d'une virgule
- Puis le numéro d'inventaire


<a id='t4-12'/>

## Métadonnées DC : identificateur

Le champ **Identifier** de Dublin Core préconise d'indiquer ici des identifiants techniques univoques, comme l'ISBN pour un livre.

Dans le contexte, on peut y mettre un lien vers la notice du document sur le site de l'institution conservatrice :

- S'assurer que l'on copie un permalien… (l'URL se termine généralement par un code d'identification)
- Le coller dans Tropy


<a id='t4-13'/>

## Métadonnées DC : format

**Format** désigne la manifestation (ou matérialisation) physique ou numérique de la ressource.

Il est recommandé d'y indexer le type de médium, de support ou les dimensions de l'objet.

- Accéder au thésaurus de l'INHA **Techniques**, [\textcolor{blueici}](https://thesaurus.inha.fr/thesaurus/page/ark:/54721/05085df9-7b57-4aca-b600-fa0309b0cb3c) et trouver le descripteur le plus adapté et le plus précis (en cliquant sur les termes pour descendre dans la hiérarchie)

<!--
Le plus pertinent, peinture à l'huile, se trouve dans "technique picturale (liant)" :
https://thesaurus.inha.fr/thesaurus/page/ark:/54721/827a1923-2d1e-4731-adcd-b3d1cee5536f
-->


<a id='t4-14'/>

## Métadonnées DC : format

On peut ajouter un second champ format :

- Clic droit sur les métadonnées > **Nouveau champ**
- Saisir `Format`

On peut aussi, plus simplement, inscrire plusieurs valeurs dans le champ unique Format et les séparer par des virgules :

- Accéder au thésaurus de l'INHA **Matériaux**, [\textcolor{blueici}](https://thesaurus.inha.fr/thesaurus/page/ark:/54721/2275eb81-6e47-4c3c-b1ee-96795edb046c) et trouver le descripteur…


<a id='t4-15'/>

## Métadonnées DC : sujet, couverture

- **Sujet** : concerne l'indexation du contenu thématique de la ressource
	
	- Tropy associe plus efficacement un volet de **Tags**
	- On peut y saisir les termes renseignés dans la partie *Indexation* de la notice du musée, mais attention : on ne veut pas se retrouver noyé sous les *tags* ; ils doivent vous servir avant tout à créer des liens entre les objets en fonction de vos questionnements de recherche
	- Indexer comme tag l'œuvre littéraire dont la peinture est inspirée :

		- Le meilleur thésaurus d'œuvres littéraires, comme *Les Fourberies de Scapin* : [\textcolor{blueData-BNF}](https://data.bnf.fr/)

- **Couverture** (*coverage*) : permet de compléter l'indexation en désignant une notion spatio-temporelle

	- Période
	- École artistique, etc.


<a id='t4-16'/>

## Métadonnées DC : autres

Champs moins utiles ou non pertinents pour cette œuvre :

- Collaborateur :
	- *Pour une estampe* : le graveur (si différent du dessinateur)

- Editeur (*Publisher*)
	- *Pour une estampe* : le libraire-éditeur qui la commercialise

- Rights
- Langue
- Relation : 
	- *Pour une archive* : on mettrait ici le lien vers la notice dans l'inventaire de recherche


<a id='t4-17'/>

## Indexer une lithographie parue dans la presse


**Image** : [*Les conseils d'un Crispin politique*](img/charivari-1851-05-12_bpt6k3057446h_f3.jpg)


- Naviguer jusqu'au dossier  `bib-num\sources\presse\charivari…`
- Importer l'image dans Tropy
- Renseigner les champs DC en vous aidant du lien [\textcolor{blueGallica}](https://gallica.bnf.fr/ark:/12148/bpt6k3057446h/f3)
- **Source** est ici à utiliser pour la référence de la publication
- **Date** : privilégier le format ISO ainsi : `1851-05-12`


<a id='t4-18'/>

## Indexer une lithographie parue dans la presse

**Analyser l'objet**

Si l'on double-clique sur l'œuvre :

- On peut associer des **notes** à l'objet dans son ensemble
- Ou encore, avec l'**outil de sélection** placé au dessus de la reproduction, définir des **zones d'intérêt**, et rédiger une note pour chacune


<a id='t4-19'/>

## Indexer un document d'archive


**Image** : [Lettre autographe de Daumier](img/autographes-10_0646_doucet_aumf04c010_000458.jpg)


- Naviguer jusqu'au dossier  `bib-num\sources\archives\`\
	`paris-binha-doucet\autographes-10\`
- Importer l'image dans Tropy
- Renseigner les champs DC en vous aidant du lien vers la [\textcolor{bluebibliothèque numérique de l'INHA}](https://bibliotheque-numerique.inha.fr/collection/item/17261-autographes-carton-10-peintres-cou-dav)
- *Type* : DC recommanderait `text` ; mais on peut être plus précis et créatif (correspondance, autographe…)
- *Source* : la cote complète de l'archive


<!--
photo
https://bibliotheque-numerique.inha.fr/viewer/17261/?offset=#page=458
-->

<a id='t4-20'/>

## Transcrire un document en note


**Image** : [Lettre autographe de Daumier](img/autographes-10_0646_doucet_aumf04c010_000458.jpg)


- Entrer dans l'objet
- **Etablir la transcription** du document dans une note
- Tenter d'identifier les personnes citées dans la lettre\
	 On apprend grâce à l'index du catalogue *Daumier, 1808-1879*, dir. H. Loyrette (Paris, 1999) que Daumier fréquentait un certain `Boissard de Boisdenier, Joseph-Ferdinand`

- Créer un *tag* à partir de la notice de cet artiste sur [\textcolor{blueULAN}](https://www.getty.edu/research/tools/vocabularies/ulan/)


<!--
ULAN : http://vocab.getty.edu/page/ulan/500002694
-->

<!--

<a id='t4-21'/>

## Grouper les objets par listes

-->


<a id='t4-22'/>

## Fermer et rouvrir le projet


Mission terminée !


Le projet est conservé dans un `dossier.tropy`

Pour l'ouvrir à nouveau :

- Entrer dans le dossier
- Double-cliquer sur le fichier `.tpy`