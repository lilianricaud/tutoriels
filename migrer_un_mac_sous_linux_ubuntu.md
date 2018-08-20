<!--

---
title: Migrer un mac sous Linux Ubuntu
description: Voici comment j'ai très simplement migré mon mac sous linux Ubuntu.
image_url:
licence: CC-BY-SA 
---

-->


# Migrer un mac sous Linux Ubuntu

Voici comment j'ai très simplement migré mon mac sous linux Ubuntu.

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

Voir la liste des logiciels dans le tuto PRODUCTIVITÉ SUR UBUNTU.



### Bug clavier

Note sur un bug assez enervant: le curseur de la souris sautait enormément lors de la frappe au clavier.

Après desinstallation du pilote de pavé tactile Synaptics pour le serveur X.Org ("xserver-worg-input-synaptics" effectué dans la logithèque) et réinstallation avec le greffon optionnel "dispositif de pointage" (gpointing-device-settings). tout semble marcher.

source: https://forum.ubuntu-fr.org/viewtopic.php?id=310542
