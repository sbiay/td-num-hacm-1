---
mainfont: Alegreya
title: Générer un catalogue d'œuvres à partir d'une collection de fichiers
date: 1^er^ semestre 2025-2026
author: sebastien.biay@univ-nantes.fr
lang: fr-FR
header-includes: 
	- \usepackage[font=small,justification=centering]caption
---

Générer un catalogue d'œuvres à partir d'une collection de fichiers
=====

Plan :

	1. [Méthode](#t0-1)
	2. [Méthode](#t0-2)
1. [Le langage markdown](#t1)
	1. [Langages à balises](#t1-1)
	2. [Avantages du markdown](#t1-2)
	3. [Prérequis](#t1-3)
	4. [Editer un document](#t1-4)
	5. [Parties du document](#t1-5)
	6. [Styles de paragraphes](#t1-6)
2. [Titre de niveau 1](#t2)
	1. [Titre de niveau 2](#t2-1)
	2. [Styles de paragraphes](#t2-2)
	3. [Styles de paragraphes](#t2-3)
	4. [Styles de caractères](#t2-4)
	5. [Styles de caractères](#t2-5)
	6. [Liens et images](#t2-6)
	7. [Liens et images](#t2-7)
	8. [Liens et images](#t2-8)
	9. [Liens et images](#t2-9)
	10. [Notes](#t2-10)
	11. [Notes](#t2-11)
	12. [Notes](#t2-12)
	13. [Notes](#t2-13)
	14. [Commentaires](#t2-14)
	15. [Transformer un fichier md en traitement de texte](#t2-15)
3. [Réaliser un catalogue de notices](#t3)
	1. [Structure des notices](#t3-1)
	2. [Structure des notices](#t3-2)
	3. [Structure des notices](#t3-3)
	4. [Créer une nouvelle notice](#t3-4)
	5. [Créer une nouvelle notice](#t3-5)
	6. [Préparer les pages de titre du catalogue](#t3-6)
	7. [Rédiger la commande pandoc](#t3-7)
	8. [Rédiger la commande pandoc](#t3-8)
	9. [Rédiger la commande pandoc](#t3-9)
	10. [Rédiger la commande pandoc](#t3-10)
	11. [Rédiger la commande pandoc](#t3-11)
	12. [Rédiger la commande pandoc](#t3-12)
	13. [Mettre en forme le catalogue](#t3-13)
	14. [Mettre en forme le catalogue](#t3-14)
4. [Créer une collection Omeka](#t4)
	1. [Extraire les données Dublin Core des notices](#t4-1)
	2. [Extraire les données Dublin Core des notices](#t4-2)
	3. [Extraire les données Dublin Core des notices](#t4-3)
	4. [Charger les données dans une collection Omeka](#t4-4)
	5. [Charger les données dans une collection Omeka](#t4-5)
	6. [Charger les données dans une collection Omeka](#t4-6)
	7. [Charger les données dans une collection Omeka](#t4-7)
	8. [Charger les données dans une collection Omeka](#t4-8)

<!--FINET-->


<a id='t0-1'/>

## Méthode
[comment1]: <2> (TITRE1)

**Image** : [Flux de production classique](img/catalogue_schema1.png)


<a id='t0-2'/>

## Méthode

**Image** : [Flux de production à double sortie](img/catalogue_schema2.png)


<a id='t1'/>

# Le langage markdown
[comment2]: <3> (TITRE1)

<a id='t1-1'/>

## Langages à balises


```html
<!DOCTYPE html>
<html>
	<head>
		<title>Une petite page HTML</title>
	</head>
	<body>
		<h1>Un titre de niveau 1</h1>
		<p>Un premier petit paragraphe.</p>
	 
		<h2>Un titre de niveau 2</h2>
		<p>
			Un autre paragraphe contenant un lien pour aller
			sur le site <a href="http://koor.fr">KooR.fr</a>
			pour apprendre à écrire du HTML.
		</p>
	</body>
</html>
```

<a id='t1-2'/>

## Avantages du markdown

- Syntaxe simple à comprendre
- Rapidité de saisie
- Lisible, même sans prévisualisation
- Portabilité des fichiers : texte brut, léger, consultable sur tous les éditeurs, dans toutes les OS
- Flexibilité du contenu : conversion possible dans de multiples formats
- Très largement utilisé dans les systèmes de gestion de contenu (bases de données, blogues scientifiques, etc.)


<a id='t1-3'/>

## Prérequis

Pour rédiger en md, on utilise un **éditeur de texte** et non un logiciel de traitement de texte :

- [\textcolor{blueVisual Studio Code}](https://code.visualstudio.com/download)
- [\textcolor{bluePulsar}](https://pulsar-edit.dev/download/)
- Et tant d'autres à découvrir [\textcolor{blueici}](https://www.logiciels.pro/comparatif-logiciels/comparatif-editeurs-markdown/)

Installer [\textcolor{blueVisual Studio Code}](https://code.visualstudio.com/download) et le démarrer


<a id='t1-4'/>

## Editer un document

- Télécharger le dossier **daumier.zip** depuis Madoc
- Extraire le contenu
- Ouvrir Visual Studio
- Dans le volet d'exploration (Ctrl + Maj + E), ouvrir le dossier `daumier`
- Naviguer via le volet d'exploration jusqu'au fichier 
	`.\bib-num\etudes\loyretteDaumier18081879Cat1999\notes.md`
- L'ouvrir
- Fermer le chat à droite
- Cliquer sur le bouton de prévisualisation en haut à droite (icône en forme de double page avec une loupe)


<a id='t1-5'/>

## Parties du document

- **En-tête** : les métadonnées du document au format Yaml

	- Certains caractères sont interdits, comme `:`
	- `lang: fr-FR`  est très important pour une transformation selon des règles typographiques françaises (appel de note avant la ponctuation) 

- **Corps** du document


<a id='t1-6'/>

## Styles de paragraphes

**Titres**\
Le symbole `#` permet de baliser une ligne de titre\

```md
<a id='t2'/>

# Titre de niveau 1
<a id='t2-1'/>

## Titre de niveau 2
```

À faire :

- Faire passer `Théâtre, Molière` en titre de niveau 1
- `Cat. 204 Crispin et Scapin` en titre de niveau 2


<a id='t2-2'/>

## Styles de paragraphes

**Paragraphe standard**\
Le retour à la ligne n'interrompt pas un paragraphe\
Seule une ligne vide marque une séparation entre deux paragraphes :

- Remarquer que la phrase `Oeuvre bien conservée…` est écrite sur plusieurs lignes
- Remplacer les retours à la lignes par des espaces : la prévisualisation du document n'est pas affectée

On force un retour à la ligne avec `\` :

- Placer `\` au bout de la ligne `Identification du sujet :`


<a id='t2-3'/>

## Styles de paragraphes

**Blocs de citation**\
Le symbole `>` permet de baliser un bloc en retrait\

- A la fin du fichier, placer `>` (suivi d'une espace) devant `Degas admira` et devant `A Daumier`


<a id='t2-4'/>

## Styles de caractères

**Italique**\
Le symbole `*` permet de baliser une chaîne de caractères en italique :

- Ligne 23, saisir un `*` avant `Fourberies` et après `Scapin`
- On peut aussi sélectionner les mots (Ctrl + Maj + flèche) et appuyer une seule fois sur `*`
- Faire de même pour `Scapin et Silvestre`

<a id='t2-5'/>

## Styles de caractères

**Gras**\
Les symboles `**` permettent de baliser une chaîne de caractères en gras :

- Sélectionner `Identification du sujet` et saisir `**`


**Gras et italique**\
Les symboles `***` permettent de baliser une chaîne de caractères en gras et en italique


<a id='t2-6'/>

## Liens et images

**Liens hypertextes**\
Pour insérer un lien :

- Sélectionner le texte support du lien : `portail des collections d'Orsay`
- Saisir `[` pour l'enfermer dans des crochets carrés
- Après `]` saisir des parenthèses simples `()`
- Placer entre les parenthèses [\textcolor{bluecette URL}](https://www.musee-orsay.fr/fr/oeuvres/crispin-et-scapin-10867)


<a id='t2-7'/>

## Liens et images

**Images**\
Pour insérer une image :

- Sous le Titre 2, sauter une ligne et saisir `![]()`
- Le texte de la légende s'écrit entre `[]`
- L'[\textcolor{blueURL de l'image}](https://cdn.mediatheque.epmoo.fr/link/3c9igq/bez1butv71h3w00.jpg) s'écrit entre `()`

On peut également insérer un fichier-image local par son chemin absolu :

- Dans le volet de navigation de Visual Studio > clic droit sur le fichier visé > **Copy Path**

- Le coller dans le fichier md à la place de l'URL de l'image


<a id='t2-8'/>

## Liens et images

**Images citées par URL** :

- Prévisualisation md
- Export direct vers le catalogue traitement de texte\
	(via pandoc)
- Export direct vers Omeka (via CSV)

**Images citées par chemin absolu** :

- \textcolorpurpleNe permet pas la prévisualisation md
- Export direct vers le catalogue traitement de texte\
	(via pandoc)
- \textcolorpurpleNe permet pas l'export direct vers Omeka (via CSV)

<a id='t2-9'/>

## Liens et images

**Format des images**\
afin d'éviter que des images de grand format ne débordent de la page lors d'une transformation vers traitement de texte,
indiquer en bout de ligne une dimension maximale :

- `{ width=16cm }` pour une image de format paysage
- `` pour une image de format portrait


<a id='t2-10'/>

## Notes

L'insertion de notes accepte plusieurs syntaxes

**Syntaxe principale**

- Insérer l'appel de note après `J. Adhémar` de la façon suivante : `[^<!---->1]`
- Créer la note sur une nouvelle ligne (précédée et suivie par une ligne vide) :
	
	- `[^<!---->1]: J. Adhémar, *Honoré Daumier*, Paris, P. Tisné, 1954, p. 126.`

Attention copier/coller le caractère `^` peut ne pas fonctionner\
La numérotation des notes accepte les chiffres comme les lettres


<a id='t2-11'/>

## Notes

**Syntaxe alternative**

`Du texte^[Le contenu d'une note].`

- \textcolorpurpleNe permet pas la prévisualisation md
- Export direct vers le catalogue traitement de texte\


**Syntaxe principale**

- Prévisualisation md
- \textcolorpurpleLes notes qui auraient le même numéro ne peuvent pas être fusionnées via pandoc


<a id='t2-12'/>

## Notes

Transformer l'ensemble des indications de pagination en notes avec la clé de citation **BetterBibTeX** (qu'il faut d'abord configurer) :

- Ouvrir Zotero et se connecter à son compte
- Se rendre sur la page de téléchargement de BetterBibTex pour Zotero [\textcolorblueici](https://github.com/retorquere/zotero-better-bibtex/releases/latest)

	- Cliquer droit sur le fichier **.xpi** pour l'enregistrer sous
	- Dans Zotero : **Outils** > Extensions
	- Cliquer sur la **roue dentée** > Install plugin from file

- Copier la clé de citation `loyretteDaumier18081879Cat1999`


<a id='t2-13'/>

## Notes

Dans le fichier de notes :

- Ouvrir la boîte de dialogue de cherche-remplace (Ctrl + H) :
- Activer les expressions régulières : `.*`
- Rechercher : `\s\[(p.\s\d+)\]`
	- `\s` : caractère blanc (espace ou tabulation --- *space*)
	- `\d` : chiffre (*digit*)
- Remplacer par :\
	`^[loyretteDaumier18081879Cat1999, $1.]`

Attention copier/coller le caractère `^` peut ne pas fonctionner\


<a id='t2-14'/>

## Commentaires

Pour saisir des informations qui ne seront pas visibles dans la prévisualisation ou lors de l'export vers le catalogue traitement de texte :

\<\!\-\-Du texte en commentaire sur une ligne\-\-\>

\<\!\-\-\
Du texte en commentaire\
sur plusieurs lignes\
\-\-\>\


<a id='t2-15'/>

## Transformer un fichier md en traitement de texte

**Pandoc**\
est un logiciel de transformation en ligne de commande (pas d'interface utilisateur) :

- Déjà installé en salle informatique\
	
	pour l'installer chez soi, le télécharger [\textcolor{blueici](https://pandoc.org/installing.html) (au format **msi** pour une bonne installation sous Win)
	
- Dans le volet de navigation Visual Studio cliquer droit sur le dossier `loyretteDaumier18081879Cat1999` > Open in integrated Terminal

- Écrire (ou copier-coller) la commande suivante :\
	`pandoc .\notes.md -o sortie-traitnt-txt.odt`\

- Ouvrir le résultat dans LibreOffice Writer


<a id='t3'/>

# Réaliser un catalogue de notices
[comment3]: <24> (TITRE1)

<a id='t3-1'/>

## Structure des notices


- Avec le volet de navigation, accéder au dossier `bib-num\sources\presse\charivari-1851-05-12`
- Ouvrir le fichier `notice.md`

Il contient tous les éléments constitutifs d'une notice :

-  Image
- Données catalographiques
- Bibliographie (les données ne sont pas authentiques)
- Brève analyse

Et des éléments de structure :

-  Titre 2 pour la notice dans son ensemble, qui prendra la forme d'une numérotation qui sera écrite automatiquement (par exemple `Cat. 1`)
- Titre 3 pour séparer l'analyse dans le futur catalogue
- Ne rien écrire dans ces titres !
- On réserve le niveau Titre 1 pour les titres des grandes parties du catalogue : Estampe, Peinture, etc.

<a id='t3-2'/>

## Structure des notices

Les notices contiennent également des **balises HTML**

`<data name="DC.creator">CONTENU</data>`

Elles permettront plus tard de récupérer automatiquement le contenu saisi dans ces balises et de les convertir en un tableau de données au format CSV

Les données seront envoyées vers le logiciel Omeka qui demande qu'elles soient exprimée selon le modèle **Dublin Core**


<a id='t3-3'/>

## Structure des notices

L'intitulé des données catalographiques (artiste, titre, technique, etc.) n'est pas toujours écrit à l'intérieur de la balise `<data…`

En l'écrivant parfois à l'extérieur de la balise, on évitera de l'exporter vers la collection virtuelle Omeka, où les intitulés des champs Dublin Core sont écrits et risqueraient d'être redondants (avec notamment titre, date, source)

Voir la notice Omeka [\textcolor{blueici](https://duelsbiay.omeka.net/items/show/218)


<a id='t3-4'/>

## Créer une nouvelle notice

En vous inspirant de cette notice modèle, créer et renseigner une nouvelle notice :

- Avec le volet de navigation, accéder au dossier `.\bib-num\sources\presse\charivari-1865-06-24\`
- Récupérer le formulaire vierge **notice.md** sur Madoc et le placer dans ce dossier
- En vous aidant du modèle et de la notice Gallica [\textcolor{blueici](https://gallica.bnf.fr/ark:/12148/btv1b525144764/f1)


<a id='t3-5'/>

## Créer une nouvelle notice

Les plus rapides créeront aussi une notice pour cette œuvre :

`.\collections\france\paris-louvre\amateurs-estampes-RF-4036\`


<a id='t3-6'/>

## Préparer les pages de titre du catalogue

Ce sont les titres 1 qui constitueront les titres des grandes parties du catalogue

Pour chacun, on a créé un fichier md qui se trouve à la racine du dossier `daumier` :

- partie1-estampe.md
- partie2-dessins.md
- partie3-peinture.md

On a également créé un fichier **metadonnees.md** qu'il faut à présent compléter des informations à faire apparaître sur la pièce de titre du catalogue


<a id='t3-7'/>

## Rédiger la commande pandoc

Pour transformer avec **Pandoc**, il faut rédiger une ligne de commande comme précédemment :

`pandoc .\notes.md -o sortie-traitnt-txt.odt`

Mais on doit désormais indiquer en 1^er^ argument\
(entre `pandoc` et `-o`)\
l'ensemble des fichiers qui composent le catalogue
**dans l'ordre souhaité**

<a id='t3-8'/>

## Rédiger la commande pandoc


- Créer un fichier **commande-pandoc.txt**\
	dans le dossier **daumier**\
	C'est possible dans le volet de navigation, par un clic droit
- L'ouvrir dans Visual Studio Code
- Inscrire dans ce fichier, ligne après ligne :

	```txt
	pandoc
	metadonnees.md
	partie1-estampe.md
	```

<a id='t3-9'/>

## Rédiger la commande pandoc

- Pour inscrire le chemin de fichier de chaque notice dans l'ordre souhaité : 
	
	- Dans l'explorateur de fichiers Windows, se placer dans le dossier `daumier`
	- Rechercher **notice.md**
	- Cliquer gauche sur le premier fichier que l'on veut insérer dans le catalogue
	- Ctrl + C
	- Coller à la suite du document **commande-pandoc.txt** 

		`bib-num/sources/presse/charivari-1851-05-12/notice.md`\
		`bib-num/sources/presse/charivari-1865-06-24/notice.md`

<a id='t3-10'/>

## Rédiger la commande pandoc

Une fois toutes les notices ajoutées, la dernière ligne de la commande est :

`-o catalogue.odt`


<a id='t3-11'/>

## Rédiger la commande pandoc

Il faut à présent transformer l'ensemble des lignes en une seule ligne.
On conserve la version écrite sur plusieurs lignes car il est facile d'en modifier l'ordre au besoin :

- Dans Visual Studio, ouvrir un document brouillon\
	(Ctrl + N)
- Copier-coller toutes les lignes de **commande-pandoc.txt**
- Ouvrir le dialogue cherche-remplace (Ctrl + H)
- Activer les expressions régulières
- Chercher les retours à la ligne : `\n` (*newline*)
- Remplacer par une espace
- Copier-coller le résultat en bas du fichier **commande-pandoc.txt** (ne pas supprimer le reste)


<a id='t3-12'/>

## Rédiger la commande pandoc

Pour finir, lancer pandoc avec la commande :

- Cliquer droit sur le volet de navigation : **Open in integrated Terminal**

- Copier-coller toute la commande en une ligne, puis **Entrée**

- Ouvrir le résultat dans LibreOffice Writer

- Contrôler que tous les éléments se trouvent dans le fichier, dans le bon ordre


<a id='t3-13'/>

## Mettre en forme le catalogue

Comme le catalogue à l'état brut contient déjà des styles de paragraphes, on peut lui appliquer une mise en forme prédéfinie à partir d'un document modèle…

- Télécharger le fichier **catalogue.odt**
- L'ouvrir, puis en sauvegarder le modèle
- **Fichier** > Modèles > Enregistrer comme modèle
- Sélectionnez la catégorie du modèle : **Styles**
- Nommer le modèle : `catalogue`

Dans votre propre catalogue odt :

- **Styles** > Charger des styles depuis un modèle
- Bien cocher toutes les cases, notamment :

	- Page
	- Ecraser

<a id='t3-14'/>

## Mettre en forme le catalogue


Félicitations !


Vous avez généré un catalogue d'œuvres à partir d'un lot de fichiers.


<a id='t4'/>

# Créer une collection Omeka
[comment4]: <38> (TITRE1)

<a id='t4-1'/>

## Extraire les données Dublin Core des notices
[comment5]: <39> (TITRE2)

Pour extraire les données inscrites dans les balises `<meta…` des notices, on utilise un script en langage python : **extraction-donnees.py**

Python est installé sur les PC de la salle informatique et on peut l'utiliser via le terminal de Visual Studio Code


<a id='t4-2'/>

## Extraire les données Dublin Core des notices


Pour installer python sur un ordinateur personnel, je conseille la suite Anaconda à télécharger [\textcolor{blueici](https://www.anaconda.com/download/success)

- Une fois installé, lancer Anaconda Powershell Prompt
- Installer les expressions régulières avec la commande\
	`conda install regex`
- Se déplacer dans le dossier de travail à l'aide de la commande **cd** (*change directory*) ; pour comprendre les principales commandes, dont cd, voir [\textcolor{bluece tutoriel](https://tutorials.codebar.io/command-line/introduction/tutorial.html)


<a id='t4-3'/>

## Extraire les données Dublin Core des notices

Toujours dans le terminal positionné dans le dossier `daumier`, saisir la commande :

- On commence par installer un module nécessaire à la future transformation :\

	```shell
	pip install regex
	```
- Une fois l'installation faite, on passe la commande :

	```shell
	python extraction-donnees.py
	```

Il suffit d'écrire `python ext` puis d'appuyer sur la touche **Tab** pour profiter de l'autocomplétion, puis Entrée


<a id='t4-4'/>

## Charger les données dans une collection Omeka

**Omeka**\
Est un CMS (*content manager system*) open source

Accéder à la page d'[\textcolor{blue{accueil](https://www.omeka.net) et se créer un compte gratuit

On peut tout aussi gratuitement créer 1 site avec 500 MB de stockage

Créer votre site : je vous conseille d'utiliser votre nom ou un mot lie à votre recherche pour en définir l'adresse


<a id='t4-5'/>

## Charger les données dans une collection Omeka

À partir de l'écran d'administration du site :

- Dans le menu en haut de l'écran
- Plugins > CSV Import > Install
- Appearance : choisir un thème
- Settings : on peut renseigner les informations sur le site, notamment le **Site Title**


<a id='t4-6'/>

## Charger les données dans une collection Omeka

Cliquer sur CSV import dans le menu de droite

- Upload CSV File : aller chercher votre fichier CSV via **Parcourir**
- Make All Items Public : **cocher**
- Choose Element Delimiter : `|` (Alt Gr + 6)
- Passer à l'étape suivante


<a id='t4-7'/>

## Charger les données dans une collection Omeka

- Pour chaque ligne (sauf la dernière, *File*), ouvrir le menu **Map to element** et choisir le type de donnée indiqué dans la colonne de gauche

- Cocher la case **Use HTML** dans les cas suivants :

	- Format
	- Source
	- Description
	- Description-bib
	- Publisher
	- Type

- Cocher la case **Files** pour la dernière ligne


<a id='t4-8'/>

## Charger les données dans une collection Omeka


Félicitations !


Vous savez maintenant comment créer une collection virtuelle avec votre corpus de recherche