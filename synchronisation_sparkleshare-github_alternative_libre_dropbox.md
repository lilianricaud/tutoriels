<!--

---
title: Synchroniser un dossier local avec github en 5 min grace au logiciel Sparkleshare
description: Dans ce tutoriel je décris comment syncrhoniser en 5 minutes un dossier local sur votre ordinateur et un repertoire Github. Ceci se fait via l'installation et l'utilisation du logiciel SparkleShare. Pour les commoners qui souhaitent mutualiser leurs publication, ceci permet un usgae de type dropbox où on travaille en local et les contenus sont ensuite synchronisés avec Github et affichables sous MultiBAO.
image_url:
licence: CC-BY-SA 
---

-->


# Utilisation de Sparkleshare avec Github

Dans ce tutoriel je décris comment synchoniser en 5 minutes un dossier local sur votre ordinateur et un repertoire Github. Ceci se fait via l'installation et l'utilisation du logiciel SparkleShare. Pour les commoners qui souhaitent mutualiser leurs publication, ceci permet un usgae de type dropbox où on travaille en local et les contenus sont ensuite synchronisés avec Github et affichables sous MultiBAO.

Dans mon cas, ceci me permet d'éditer des fiches recettes sur mon bureau linux avec un simple éditeur texte et d'avoir une publication automatique en ligne sur github et multibao où elles peuvent être consultées, copiées ou enrichies par d'autres sans nécessiter aucun travail supplémentaire de ma part.

## Usage

Sparkleshare est un logiciel libre qui permet de synchroniser automatiquement des dépots entre github, bitbucket ou autres instances Git et un dossier local sur un ordinateur, agissant effectivement comme une sorte de dropbox version Git.

Il est ainsi possible de modifier localement ses fichiers markdown via un éditeur texte (Gedit reconnait markdown et marche tres bien sous ubuntu) et de travailler localement tout en ayant une sauvegarde cloud automatique sur github lorsque l'on est de nouveau connecté.

Avantage de Sparkleshare: la synchro se fait automatiquement et simplement. Interface graphique pour utiliser git/github sans ligne de commande. Seul logiciel testé qui fonctionne sous ubuntu/linux 32 bit.

Inconvénients: peu d'options, impossible de gérer des branches parallèles, des modifications à plusieurs via le logiciel.

Sparkleshare marche donc bien pour mutualiser facilement des contenus vers Github et donc MultiBAO, moins pour un travail collaboratif poussé.

## Installation

- Télécharger Spakleshare: https://www.sparkleshare.org/

- Ouvrir et installer l'archive.

Dans ubuntu, une icone apparait dans la barre de menu du haut

Choisir Sparkleshare > Client ID > Copy to clipboard

Pour récupérer une clé SSH propre au logiciel.

Aller sur les réglages github

https://github.com/settings/keys

Faire "New SSH key" et copier la clé obtenue précedemment.

Sparkleshare devrait alors être autorisé à lire et écrire tous les dépots Github du compte associé.

Note: il est faut ajouter la clé SSH au niveau des réglages (settings) de l'utilisateurs, pas des réglages d'un seul dépot sinon il ne sera pas possible d'écrire sur tous les dossiers et la clés ne peut être ajoutée qu'une seule fois dans les réglages.

## Synchronisation de dossiers locaux / dépots distant Github

Dans le menu du haut aller à:

Sparkleshare > add hosted project

Il est possible de choisir un serveur personnalisé, Bitbucket, github, gitorious.

Choisir l'option dépot Github

Indiquer le nom d'utilisateur et le nom du dépot.

Par exemple "lilianricaud/travail-en-reseau"

attention a bien rentre le nom

La synchronisation devrait alors se faire avec un dossier local appellé Sparkleshare et situé dans le dossier personnel.

Note: il est nécessaire d'effectuer cette opération pour chaque répertoire à synchroniser.

## Créer un nouveau dossier

Pour ajouter un dossier, il semble nécessaire de d'abord le creer via github et ps directement sur l'ordinateur.

Pour cela, aller dans Repositories puis Cliquer sur New pour ajouter un repertoire.

Après avoir choisi le nom, cliquer l'option add Readme, sinon le dépot ne sera pas utilisable tel quel.

Refaites la manip précédente pour autoriser sparkleshare à la synchroniser



## Plus d'infos:

Aide Sparkleshare: https://github.com/hbons/SparkleShare/wiki


## Source 

CC-BY-SA Lilian Ricaud
www.lilianricaud.com
