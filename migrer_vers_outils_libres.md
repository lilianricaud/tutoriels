<!--

---
title: Migrer vers de outils libres et conviviaux 
description: Cette fiche présente un retour d'expérience de ma migration en cours vers des outils libres et conviviaux. Migration d'un Mac sous Ubuntu, migration vers des hebergeurs web éthique, degooglization.
image_url: 
---

-->


# Migrer vers de outils libres et conviviaux 

Cette fiche présente un retour d'expérience de ma migration en cours vers des outils libres et conviviaux. Migration d'un Mac sous Ubuntu, migration vers des hebergeurs web éthique, degooglization.


# Migrer un mac sous Linux

## Remplacement du disque dur

Profitant de la mort de mon disque dur, j'ai commencé ma sortie de l'écosystème fermé d'apple en passant mon macbook pro sous linux.

J'ai d'abord commencé par remplacer le disque dur défaillant par un disque SSD Samsung de 500gb.

Pour cela il a suffit de devisser le corps du macbook pro, devisser les vis maintenant le disque dur puis remplacer celui ci sur les connectiques.



## Installation Ubuntu

Pour installer Ubuntu, j'avais gravé il y a longtemps un CD d'installation ubuntu 14.04 pour 32 bit. 

J'ai inséré ce CD dans le mac et appuyé sur la touche C au démarrage afin que l'ordinateur démarrer à partir du CD, ce qui s'est fait sans problème.

A partir de la, l'installation s'est fait naturellement en suivant les instructions et réglant les paramètres de base.

En moins d'une heure le macbook pro était installé avec ubuntu et fonctionnel.

## Réglages d'Ubuntu pour Mac

Il a ensuite fallu régler le clavier pour mac, car par défaut le clavier était pour un PC (avec quelque différences pour certaines touches. Ceci s'est fait via une ligne de code qui donnait accès a de nombreux clavier pré-réglés.

J'ai identifié un clavier français pour mac book pro et installé celui ci. Apres installation il a suffit de séléctionner le réglage de la langue pour "français macintosh" et le clavier était parfaitement fonctionnel.

La plupart des raccourcis clavier marchent.

Note la touche pomme ne marche pas, et est remplace par ctrl.
Le clic droit du touchpad n'est plus fonctionnel.

## Réglage du dock/lanceur
installation du framework dotnet.

:-/

## Migration sous Ubuntu

Ubuntu propose par défaut une inteface appellé Unity qui est tres tres proche de l'interface de MacOSX et permet à un utilisateur de mac
Sous unity, il existe un équivalent du dock de macosx qui permet de gérer ses application favorites.

J'ai personnalisé celui ci avec mes applis.

- Taper les ligne de codes du tutoriel dans le terminal
- L'appli est installé, on peut la trouver via le lanceur et l'ajouter à la barre d'applications.

Lancer l'appli de bureau, entrer les codes d'acces et l'adresse du serveur, choisir les dossier à synchroniser.


## Installation d'applis ubuntu

Ceci peut se faire en ligne de code ou pour les novices via la logithèque d'ubuntu.

Certaines applis comme skype ne sont pas accessibles via la logithèque, mais directement depuis le site de l'éditeur.

Applis installées:
- libre office, gimp, était installé par défaut dans la distribution choisie d'ubuntu.
- filezilla (ftp)
- freeplane (mindmap)
- skype (videochat)
- VLC (lecteur audio/video)
- winscop (gestion comptabilité pour les CAEs)
- Zim (wiki de bureau utilisant des fichiers textes)
- audacity (edition audio)
- Thunderbird (mail)
- Gparted (partition disque dur)
- Simple scan (gestionnaire scanner)
- Sound Juicer (extracteur audio)
- Horloge gnome (chronometre)

Voir la liste des logiciels dans le tuto productivité avec ubuntu.

### Bug clavier

Note sur un bug assez enervant: le curseur de la souris sautait enormément lors de la frappe au clavier.

Après desinstallation du pilote de pavé tactile Synaptics pour le serveur X.Org ("xserver-worg-input-synaptics" effectué dans la logithèque) et réinstallation avec le greffon optionnel "dispositif de pointage" (gpointing-device-settings). tout semble marcher.

source: https://forum.ubuntu-fr.org/viewtopic.php?id=310542

# Synchronisation avec outils de cloud

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

## Migration serveur web

J'utilisais depuis 10 ans Dreamhost un hebergeur américain qui marche très bien. Mais je voulais "rapprocher" mes données et entamer une démarche de maitrise du contenu.

### Choix d'un nouvel hebergeur plus local

- Dreamhost
- OVH
- Web4all
- Ouvaton
- Zaklys

Comparaison:
Dreamhost et OVH sont de bonne qualité, cout modique, mais sont de gros hébergeurs, utilisant plusieurs datacenters internationaux. Ouvaton est le plus affiché avec une éthique, mais qualité limité, cout élevé. Web4all ets une association qui developpe une partie de son infrastucture et s'appuie sur une infrastructure tierce (utilise des serveurs chez OVH et d'autres, privilégie hebergement en france avec partenaire français et s'appuie sur des tunnels VPN pour faire transiter les données de manière sécurisée.

Autre avantage pour Web4all, utilise Zimbra pour la gestion des mail (solution open source) ce qui semble un point fort pour faciliter la bascule depuis google. le cout est plus élevé que les autres hebergeurs (à part Ouvaton), mais reste correct.

Test 3 mois offre de base (10 sites web, 25 comptes mails): 18€ TTC

Zaklys: associatif + cloud pas cher + mail (webmail roundcube) https://cloud.zaclys.com/

## Migration site web

Après avoir longtemps hésité j'ai choisi de migrer chez ouvaton, coopérative d'hébergement basée en France avec des valeurs et une éthique forte autour de l'humain, l'autonomie et le libre (Ouvaton est dans une démarche de mise en place de CHATONs framasoft)

Etapes de Migration site web

- creer espace web pour le nom domaine chez ouvaton
- faire une sauvegardes des fichiers de mon site web avec filezilla
- faire une sauvegarde de la base de données mysql (format .sql et compression gzip) via PhpMyAdmin
- charger les fichiers du site web dans l'espace ftp ouvaton
- importer la base de données dans le PhpMyAdmin ouvaton.
- modifier les DNS chez le registrar (gandi) pour pointer vers ouvaton (ns1.ouvaton.coop, ns2..., ns3...)

## Migration mail

Voir QUITTER GMAIL dans le même dépot.






