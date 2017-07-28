<!--

---
title: Partager des ressources comme communs sur MultiBAO
description: Ce tutoriel décrit pourquoi et comment rendre partageables et interopérables des contenus libres avec Github/MultiBAO.
image_url: 
licence: CC-BY-SA
---

-->


# Partager des ressources comme communs sur MultiBAO

Ce tutoriel décrit pourquoi et comment rendre partageables et interopérables des contenus libres avec Github/MultiBAO.
image_url: 

## Avant de démarrer. 

### Le problèmes de silos

A l'heure actuelle même s'il existe beaucoup de contenus libres, en pratique ceux ci sont dur à réutiliser, car "enfermés dans des formats différents (page web au format html, pages wikis avec syntaxe wiki, fichiers docx ou odt, ...)

### A propos de Multibao

Multibao est une tentative de faciliter un réel partage de contenus sans recréer des silos.

Multibao est une sorte de lecteur qui va aller chercher des contenus stocké à différents endroits et les afficher ou les réexporter à différents endroits.

Pour cela multibao s'appuie sur une format particulier appellé **markdown**.

### A propos de markdown

Markdown est une façon de formatter des contenus (titre niveaux 1, 2...), gras, italique, listes à puces... de manière simple. 

Pour mettre un titre au format niveau 1 on mettre un dieze devant, pour un titre niveau 2 on mettre deux diezes, ... pour une liste à puces on mettre des tirets ou des étoiles pour chaque puces.

Pour lde détails des balises à utiliser voir:
https://fr.wikipedia.org/wiki/Markdown

Le format Markdown est reconnu par github, Multibao et tout un tas d'autres outils capables d'afficher le contenus de manière formatté. Il est ainsi possible d'exporter le contenu d'un pad ou d'un fichier docx en markdown ou bien de convertir un fichier markdown en HTML, en PDF ou epub.

Si markdown n'est pas un standard, il est très utilisé, peut etre facilement lu et écrit par des amateurs, des développeurs, des logiciels.

L'intéret et permettra de partager plus facilement nos contenus dans une forme facile à réutiliser par toustes.

### A propos de Github

Github est un outils tres utilisé par les développeurs pour partager du code de logiciel. Nous détournons son usage pour l'utiliser comme une base de données "ouverte", c'est à dire sans besoin de mot de passe.

Il est possible de metre tout type de contenus sur Github: PDF, images, fichiers textes au format docx ou odt, mp3s...

Ce qui nous interesse est de mettre des fichiers sous un format un peu spécial appellé markdown.



## Etape 1 : Créer des contenus markdown

### En partant de zéro

Utiliser un traitement de texte, ajouter des balises, ne pas oublier de mettre l'extension .md après le nom du fichier.



### A partir d'un fichier Word (doc ou docx)

Utiliser le service  Word to Markdown :  http://word-to-markdown.herokuapp.com/

charger votre fichier et copier coller le contenu dans votre fichier .md


## Etape 2 :  mettre ses contenus sur Github

- aller sur http://gihub.com
- Creer un compte
- Vous allze recevoir un mail pour valider votre inscription

Faire un dépot (une sorte de dossier)
Create a repository
**Important** cocher l'option
"initialize this repository with a readme"

valider la création

Creer un fichier

-> Create new file

Vous accédez à une interface d'édition
ajouter le titre avec ".md" à la fin

sauver "commit new file"

## Etape 4: Voir se contenus sur multibao

Multibao va chercher dans github les contenus a afficher. En indiquant une adresse d'un fichier .md situé sur github, multibao va être capable de le lire par exemple le fichier:

http://www.gihtub.com/lilianricaud/tutoriels/blob/master/partager_des_ressources_communs_multibao.md

Sera visible à l'adresse suivante:

http://www.multibao.org/#lilianricaud/tutoriels/blob/master/partager_des_ressources_communs_multibao.md

**Important**: ne pas oublier de mettre un dieze avant le nom d'utilisateur.


## Aller plus loin:

### Synchroniser des dossiers locaux avec Github/multibao

Dans ce tutoriel je décris comment syncrhoniser en 5 minutes un dossier local sur votre ordinateur et un repertoire Github. Ceci se fait via l'installation et l'utilisation du logiciel SparkleShare. Pour les commoners qui souhaitent mutualiser leurs publication, ceci permet un usgae de type dropbox où on travaille en local et les contenus sont ensuite synchronisés avec Github et affichables sous MultiBAO.

- http://www.multibao.org/#lilianricaud/tutoriels/blob/master/synchronisation_sparkleshare-github_alternative_libre_dropbox.md

### Partager du contenu sur d'autres sites:




### A partir d'un site WordPress

Ce tutoriel décrit comment synchroniser en 5 minutes des contenus entre un site WordPress et Github, en vue de mutualiser des contenus présents sur un site existant et les rendre partageables et interopérables avec Github/MultiBAO.

Pour les commoners qui souhaitent mutualiser leurs publication qui sont déja sur un site WordPress existant, ceci permet en 5 minutes et sans travail supplémentaire de les partager dans une format interopérable.

- http://www.multibao.org/#lilianricaud/tutoriels/blob/master/synchronisation_wordpress-github-multibao.md
