# Prototype for the web application of the project [Gustave Roud, *Œuvres complètes*](https://www.unil.ch/clsr/home/menuinst/projets-de-recherche/gustave-roud-oeuvres-completes.html)

## About this report
This document recounts the process we followed to create a prototype for the web application of the project [Gustave Roud, *Œuvres
complètes*](https://www.unil.ch/clsr/home/menuinst/projets-de-recherche/gustave-roud-oeuvres-completes.html), directed by Daniel Maggetti and Claire Jaquier. This was a joint effort of the researchers working on the project: (in alphabetical order) Alessio Christen, Bruno Pellegrino, Elena Spadini, Julien Burri and Raphaëlle Lacord. Disclaimer: we are not front-end developers.

The prototype was completed in 2018. We knew that, before the end of the project scheduled for 2021, there will be many unforeseen developments and that our prototype could not guide entirely the actual development of the web application. Nevertheless, it was a useful accomplishment, in order to clarify our ideas and to provide a foundation for the web development.

In this report the results are shown first and, afterwards, the entire process is presented. Some parts of the report are in English and some are in French.

## Table of contents

- [References](#References)
- [Results](#Results)
- [Step 1. Analyse what already exists](#step-1-analyse-what-already-exist)
- [Step 2. Imagine the final users and create *proto-personae*](#step-2-imagine-the-final-users-and-create-proto-personae)
- [Step 3. Stories and tasks](#step-3-stories-and-tasks)
- [Step 4. Content, functionalities and sitemap](#step-4-content-functionalities-and-sitemap)
- [Step 5. Mock-ups](#step-5-mock-ups)


## References
To design a prototype for the web application, we followed the indications in the first part of:

Gulio Andreini, “How we designed Galassia Ariosto”, *UX Collective*, 9 Jan 2018, <https://uxdesign.cc/how-we-designed-galassia-ariosto-9434e2732714>.

We also found a lot of information in [UX Booth](https://www.uxbooth.com/), Wikipedia, the [Web Style Guide](https://webstyleguide.com/) by Lynch and Horton, [NN/g](https://www.nngroup.com/), the [Collectif](https://archinfo.umontreal.ca) francophone sur l’architecture de l’information.

## Results

These are the mock-ups created.

| ![Homepage](/images/Accueil.png) | ![Homepage and footer](/images/Accueil_MegaMenuPieDePage.png) |
--- | ---
| ![Parcours](/images/Parcours.png) | ![Search](/images/Recherche.png) |
| ![Texts](/images/Textes.png) | ![Cueilleurs de pommes à Monneaz 1](/images/CueilleursPommesMonneaz_p1_facs.png) |
| ![Cueilleurs de pommes à Monneaz 2](/images/CueilleursPommesMonneaz_p2_facs.png) | ![Cueilleurs de pommes à Monneaz 1](/images/CueilleursPommesMonneaz_p1_tx.png) |
| ![Cueilleurs de pommes à Monneaz 2](/images/CueilleursPommesMonneaz_p2_tx.png) | ![Le repos du cavalier](/images/ReposCavalier_facs.png) |
| ![Le repos du cavalier](/images/ReposCavalier_tx.png) | ![Préface aux Œuvres complètes de C. Colomb](/images/PrefaceColomb_facs.png) |
| ![Préface aux Œuvres complètes de C. Colomb](/images/PrefaceColomb_tx.png) | ![Préface aux Œuvres complètes de C. Colomb](/images/PrefaceColomb_comparerFacsimiles.png) |
| ![Réseau génétique de l'Aveuglement](/images/Reseau_genetique_Aveuglement.png) | 

---

## Step 1. Analyse what already exist

Each of us explored a website, taking notice of features she loves and features she hates. We focused on digital editions and used the [Catalogue of Digital Editions](https://dig-ed-cat.acdh.oeaw.ac.at/) and the [Catalog of Digital Scholarly Editions](http://www.digitale-edition.de/) to find what we were looking for.

### What we (at least some of us ...) love

**Megamenus**

Example <http://www.e-codices.unifr.ch/en>, About (in the topbar).

Because it stores a lot of information, including the sections in pages; it is well structured, using bold and lines. And it does not disappear when moving the mouse.

<img src="/step1/ecodices.png" alt="e-codices" width="200"/>


**Tradition and innovation**

Example: New York Times <https://www.nytimes.com/>.

Because it mixed elements similar to the paper edition (font, position of the articles on the page) with the mechanisms of the web (multimodaliry, image carrousel, links)

<img src="/step1/nyt.png" alt="New York Times" width="200"/>



**Facsimile and transcription**

Example <https://www.bovary.fr/folio_visu.php?folio=2951&mode=sequence&mot=>.

Juxtaposition ms/transcription, considering spatial organisation and colors.

<img src="/step1/bovary.png" alt="Bovary" width="200"/>


**Simple and intuitive navigation, organised information**

Example <https://gallica.bnf.fr/ark:/12148/btv1b53025633d>

Easy zoom (almost have the feeling of playing), well structured information tab, possibility of show or hide elements easily depending on what the user wants.

<img src="/step1/gallica.png" alt="Gallica" width="200"/>


Xanadu

Example: Présentation (3 mins): <https://www.youtube.com/watch?v=Bqx6li5dbEY>. Demo: <http://xanadu.com/xanademos/MoeJusteOrigins.html>.

Because it shows the links between the texts. But it is difficult to implement ...

<img src="/step1/xanadu.png" alt="Xanadu" width="200"/>



### What we (at least some of us ...) hate

**Changing fonts and font sizes in the same page**

Exemple: New York Times <https://www.nytimes.com/>.

Exemple: The Zibaldone Project <https://www.birmingham.ac.uk/research/activity/leopardi/projects/index.aspx>.

**Unclear menus**. Which is the difference between the tabs?

Example: Les manuscrits de Madame Bovary <http://www.bovary.fr>.

**Hovering effects**. Windows opening and covering the rest of the page.

Example: L'âge d'homme <https://lagedhomme.com/>.

**Academic homepages**. Homepage addressed to specialists with a cold and austere presentation.

Example: Jane Austen Fiction Manuscripts <https://janeausten.ac.uk/index.html>.

**Illegible URLs**.

Example: <https://dig-ed-cat.acdh.oeaw.ac.at/>.


---


## Step 2. Imagine the final users and create *proto-personae*

We first defined potential final users for our web application: academic researchers and university professors, high-school students, poetry lovers, persons interested in the local cultural heritage.

For each of these categories, we imagined a person, the *proto-persona*. They will be presented in the following step.


## Step 3. Stories and tasks

Each of our persons has a story, something that she or he wants to accomplish with our web application. To reach the goal, a series of tasks should be completed; the smallest the task, the better for the design.

Here it goes the result of steps 2 and 3. The original version include fake pictures of each person, but they can't be reproduced here. These materials are in French.

#### High-school students

![Juliette](/step2/PersonCardJULIETTE.png)

Juliette's first story:

> Travail de gymnase sur d’Air de la solitude (“Bouvreuil”). Cherche un résumé du livre, qu’elle n’a pas envie de lire. Aimerais trouver une analyse du livre, synthétique. Aimerais écouter ou lire des interviews de Roud au sujet de d’Air de la solitude. Aimerais comprendre l’utilisation des noms d’oiseaux chez Roud.

Related tasks:

> Sur la page d’accueil, cherche un onglet « Œuvres », puis « Air de la solitude ». Puis « Introduction », qui raconte l’histoire du recueil et le met en perspective, dans l’œuvre de Roud. Elle Sur la page d’accueil, onglet thématique, puis oiseaux. Elle trouve un parcours dans l’œuvre de Roud, qui parle des oiseaux. Et « Roud et la nature », et elle lit aussi « Roud et la campagne vaudoise au XXe siècle ».

Juliette's second story:

> En tant qu’étudiante au gymnase, Juliette souhaite trouver des éléments qui lui permettent de présenter « Bouvreuil » paru dans Air de la solitude. Intriguée par le titre du texte, elle souhaite comprendre pourquoi Roud a pu décider l’appeler de la sorte. Sur Wikipédia, elle apprend que ce nom d’oiseau vient du latin bovariolus qui signifie « petit bœuf », ce qui l’amène à se questionner sur le rapport de Roud aux animaux. Elle effectue donc des recherches d’autres textes qui auraient le nom d’un animal pour titre, puis tente de recouper ces informations avec des éléments de la vie de l’auteur afin de chercher d’y voir plus clair.

Related tasks:

> Recherche de la liste de tous les titres des proses poétiques de Roud (Table des matières des volumes papier ?) PUIS lecture des « Éléments biographiques » et éventuellement des parcours thématiques en lien avec la campagne, la vie rurale, etc.


#### Academic research and university professors

![Yves](/step2/PersonCardYVES.png)

Yves's first story:

> Veut comprendre comment Roud a conçu le recueil « Campagne perdue », quels textes il a réunis, pour composer son recueil. Veut trouver en parallèle, les passages du journal où cette démarche est explicitée par Roud.

Related tasks:

> Sur la page d’accueil, onglets « Œuvres », puis onglet « Campagne perdue », puis onglet « Génétique ». Accède aux différentes versions génétiques des textes, classées chronologiquement. Aimerait les télécharger, pour les projeter en cours, à ses étudiants.
> Retour à la page d’accueil, onglet œuvre de Roud, onglet « recherche de mots clefs », tape « Campagne perdue » et tombe sur tous les textes de Roud qui se rapporte à ce recueil, ainsi qu’aux mentions qui sont faites de ce texte dans le Journal.
> Aimerait trouver des infos sur la réception de Campagne perdue. Sur la page d’accueil, onglets « Œuvres », puis onglet « Campagne perdue », puis onglet « Histoire du recueil », Onglet « Réception ».


Yves's second story:

> En tant que chercheur, Yves souhaite trouver et analyser tous les textes de Roud qui ont paru dans des revues mineures afin de constater s’ils varient en fonction du contexte éditorial. Il s’attend à trouver la numérisation de ces articles, mais également des éléments qui l’informent sur la publication et leur contexte (informations sur la revue, tables des matières, page entière où figure l’article de Roud). Dans un second temps, il comparera ces articles avec ceux parus dans des revues importantes.

Related tasks:

> Recherches des articles parus dans des revues mineures dans la bibliographie OU recherche des originaux numérisés organisés en fonction des revues PUIS accès à la numérisation de la revue pour la visualisation (Cf. site Gilbert Troillet : http://www.gilbert-trolliet.ch/AnimateurCulturel). Yves serait intéressé par un article qui présenterait le degré d’implication de Roud dans les revues romandes.


![Dolly](/step2/PersonCardDOLLY.png)

Dolly's first story:

> Cherche des textes qui peuvent entrer à faire partie de son corpus pour Queer studies. A besoin de faire de recherche en plein texte et de copier/coller des passages. A besoin de savoir à qui il faut s'adresser pour les droits.

Dolly's second story:

> Elle aurait besoin d’avoir la table de matiere de La plume et le regard pour savoir qu’il y a des articles qui peuvent l'intéresser.

Related tasks:

> Trouver une bibliographie secondaire > cliquer sur les liens (articles en ligne ou numérisés) > rechercher des termes spécifiques au sein de ces articles. 
> 1) Onglets en anglais (+ bio et éventuellement parcours thématiques); 2) Bibliographie critique détaillée; 3) Lien vers d’autres sites (exemple : letempsarchives.ch) ou des documents numérisés; 4) Images en mode texte, dans lesquelles on puisse effectuer des recherches simples de mots.


#### Persons interested in cultural heritage

![Philipert](/step2/PersonCardPHILIBERT.png)

Philipert's story:

> Trouver l’onglet qui permet d’accéder à une carte interactive > cliquer sur les lieux > trouver des liens vers des textes et/ou des photos en lien avec ce lieu > au sein de ces textes, pouvoir cliquer sur les noms propres (lieux et personnes) et être redirigé sur les pages correspondantes.

Related tasks:

> Carte interactive. Liens avec photos et textes.


#### Poetry lovers

![Elise](/step2/PersonCardELISE.png)

Elise's first story:

> En tant qu’amatrice de poésie et soucieuse de sa divulgation, elle souhaiterait imprimer une sélection d’extraits de textes de Roud qui apparaissent sous forme de manuscrits définitifs (soit des originaux, soit des copies de Roud pour envoi à des proches) afin de les offrir de temps en temps à ses patients et à certains de ses amis.

Related tasks:

> Reecherches de citations de textes de Roud sur la première page du site (organisées p. ex. en fonction des saisons) PUIS trouver les manuscrits qui correspondent à ces extraits. 


Elise's second story:

> Choisir l’un des « itinéraires » proposés > découvrir des liens entre l’œuvre et la biographie, des documents numérisés, des photos.

Related taks:

>  Beaucoup de liens entre les choses. Des points de référence (ex. : Rimbaud, Ramuz) pour découvrir Roud, qu’elle ne connaît pas.


## Step 4. Content, functionalities and sitemap

We could then extract some of the suitable contents and functionalities of the web application from the stories and the tasks. Then the relations between these elements could be defined.

Navigation is a key concept here. Eventually, a sitemap was designed.

This is a non comprehensive list of contents and functionalities (in French):

- Home
	- citations qui défilent (avec lien au manuscrit et au texte)
- Pour chaque texte
	- Analyse synthétique/résumé/Mots de présentation de chaque texte
	- Quels textes sont réunis dans un recueil
	- Passages du journal en lien avec un texte
	- Réception de chaque texte
	- Génétique (documents classés chronologiquement)
	- Variantes catégorisées
	- Fac similés
	- Entités sémantiques
- Liens à d’autres ressources
	- Liens avec les interviews à Roud
	- Littérature critique (ou secondaire), assez détaillée (par exemple, table de matière des recueils d’articles, comme La plume et le regard)
	- Liens à des archives et bases de données
- Bibliographie
	- liste des entrées, avec des blocs qui s’affichent ou pas, pour organiser le contenu de la bibliographie et aussi pour voir la table des matières des recueils.
	- renvoi à l’édition papier 
- Carte interactive (zoom, Roud street view)
- Documentation
	- Informations sur les droits (pouvoir utiliser certains textes dans un corpus plus large)
- Biographie
- Index des lieux et des personnes
- Parcours thématique / Promenades
	- Roud et les oiseaux
	- Roud et la nature
	- Roud et la campagne vaudoise au XXe siècle
	- Roud et le désir homoérotique
	- La mise en recueil chez Roud
	- Roud et les étoiles
	- Roud à sa table de travail
	- Rapport avec les médias
- Fonctionalities
	- télécharger fac-similés
	- copier / coller les textes (les télécharger)
	- recherche dans tous les textes
	- comparer les versions des textes
	- trier les manuscrits selon différents critères (par exemple étape génétique, manuscrit ou dactylo, etc.)
	- carte interactive
	- site multilingue


## Step 5. Mock-ups

And eventually we drew !

The [Web Style Guide](https://webstyleguide.com/wsg3/3-information-architecture/4-presenting-information.html) (chapter 3, section 4) was particularly useful here.

The results are shown at the beginning of this report.








