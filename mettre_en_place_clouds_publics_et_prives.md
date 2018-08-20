<!--

---
title: Mettre en place des espaces clouds publics et privés
description: Voici comment j'ai comment j'ai mis en place différents espace "cloud" pour partager des documents de manièr eplus ou moins ouverte pour mutualiser et collaborer facilement tout en conservant ma vie privée. 
image_url:
licence: CC-BY-SA 
---

-->


# Mettre en place des espaces clouds publics et privés

Voici comment j'ai comment j'ai mis en place différents espace "cloud" pour partager des documents de manièr eplus ou moins ouverte pour mutualiser et collaborer facilement tout en conservant ma vie privée. 

## Synchronisation avec outils de cloud

- owncloud: https://software.opensuse.org/download/package?project=isv:ownCloud:desktop&package=owncloud-client
- cozycloud: https://docs.cozy.io/en/mobile/desktop.html
- github: https://desktop.github.com/
- google drive https://apps.ubuntu.com/cat/applications/raring/grive/

## Cloud public Github

L'idée est de rendre directement partageables et améliorables les documents destinés a être partagés et eventuellement amélioré via github utilisé à la fois comme outil collaboratif et comme cloud public.

Plusieurs outils testés, l'outil retenu est Sparkleshare qui permet une synchronisation automatique entre un dossier local et un dépot github.

### Github Desktop

Github desktop est un editeur local github
avantages interface graphique et sauvegarde locale pour travailler sur fichiers github en mode déconnecté.

Problèmes ne semble pas fonctionner sous Ubuntu et la version Windows necessite Dotnet de microsoft et ne semble pas fonctionner même après l'installation de Vine.

### Installation Git

pour synchronisation avec github, github desktop n'est pas disponible pour ubuntu et ne semble pas marcher avec l'émulateur windows.

Il semble donc necessaire de passer par git et la ligne de code.

https://www.howtoforge.com/tutorial/install-git-and-github-on-ubuntu-14.04/

Idéalement cela permettrai quand même d'avoir un copie locale de mon dépot github, qui soit elle même synchronisée en permanence avec le dépot en ligne. A verifier si cela peut se faire automatiquement.

### Synchro ligne de commande

What is the git (github)command to get all the repositories pulled to my local ubuntu machine?

1. git clone <repo url> will create a git repo on your system
2. git pull will pull and merge the remote repos in your local repos
3. git fetch origin will update the remote branch on your system(one with origin/master)
4. git rebase origin/master will update your working directory.

All these are OS independent. :)

https://www.quora.com/What-is-the-git-github-command-to-get-all-the-repositories-pulled-to-my-local-ubuntu-machine

Par défaut le dépot git local est dans le dossier racine (home) et il faut spécifier le sous dossier choisi avec la commande suivante:

cd LocalGitFolder

(voir https://www.howtoforge.com/tutorial/install-git-and-github-on-ubuntu-14.04/)

Toutes les commandes git:
https://www.unixmen.com/use-git-commands-linux-terminal/

Explication fonctionnement Git
http://rogerdudler.github.io/git-guide/index.fr.html

## Alternative à Github desktop

Après recherche il existe des alternative a github desktop qui agisse comme client graphique pour Git (donc equivalent).

- https://git-scm.com/downloads/guis

### Test Giggle

pas de documentation en ligne et aide sommaire dans le logiciel.

### Test GitEye

A l'air bien, mais prise en main complexe si on connait mal le monde git.

### Test GitKraken

Outil puissant notamment pour la gestion des branches, mais pas forcement intuitif quand on est pas familier avec git. a noter la version linux est pour uniquement pour des ordinateurs avec architecture 64 bit. :-/



### Sparkleshare

Après de nombreux essais, sparkleshare est le seul outil que j'ai pu faire fonctionner sur mon mac-ubuntu (32bit), les autres nesemblent être dispo qe pour des 64 bit.

L'outill marche tres bien pour un usage de type dropbox: on enerigistre ses fichiers en local et sparkleshare les synchronise avec le dépot github (ou bitbucket, git, ...)

Voir le tuto dans le même dossier.


## Cloud Semi public Owncloud

L'idée est d'avoir un synchro cloud qui permette à la fois d'avoir une sauvegarde et un accès via d'autres postes de travail à certains docs. Ces docs sont semi-publics c'est a dire a priori destinés a être partagés, même s'il ne sont pas public en permanence et/ou accessible sous certaines conditions.

### Installation de Owncloud

- Téléchargez le fichier d'installation 
- Uploadez le fichier d'instllation dans l'espace web qui hebergera le owncloud
- Aller à l'adresse web qui pointe sur le fichier d'installation
- Suivre instructions

Notes
- Réglages Choisir base de données MySQL, car SQLlite est découragé pour filesync

Après l'installation ne pas oublier de renseigner une adresse email pour récupererle  mot de passe. Pour cela, aller dans Menu Utilisateur>personnel (en haut a droite)

### Installation de l'appli de bureau Owncloud

https://software.opensuse.org/download/package?project=isv:ownCloud:desktop&package=owncloud-client

### NextCloud: fork Owncloud

Ce fork produit par un des fondateurs semble plus éthique et moins finance que son prédecesseur.
https://nextcloud.com/

### Batir un outil evernote synchronisé avec Zim et Owncloud

Zim est un outil de wiki de bureau très léger qui utilise des simples fichiers textes pour les pages wikis. Ces pages peuvent être liées entre elles.

J'utilise un bloc note zim qui est localisé dans le dossier synchronisé avec le serveur owncloud.

Ainsi les fichiers textes sont synchronisés entre ordinateur local et serveur à distance. Je peux travailler en mode déconnecté ou bien en ligne depuis un autre appareil, la synchronisation se fait entre les deux.

Pour faciliter la réutilisation des données, je n'utilise pas les outils de formatage du wiki (ce qui utilise une syntaxe wiki dans les fichiers textes, mais plutot du markdown qui a un aspect visuel utile et peut etre réutilise via le couple github/multibao.

