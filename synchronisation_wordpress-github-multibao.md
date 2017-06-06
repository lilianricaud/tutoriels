
<!--

---
title: Synchroniser des contenus entre un site WordPress avec Github/MultiBAO en 5 min
description: Ce tutoriel décrit comment synchroniser des contenus entre un site WordPress et Gihtub, en vue de mutualiser des contenus présents sur un site existant et les rendre partageables et interopérables avec Github/MultiBAO.
image_url: 
licence: CC-BY-SA
---

-->

# Synchroniser des contenus entre un site WordPress et Github/MultiBAO 

Ce tutoriel décrit comment synchroniser en 5 minutes des contenus entre un site WordPress et Github, en vue de mutualiser des contenus présents sur un site existant et les rendre partageables et interopérables avec Github/MultiBAO.

Pour les commoners qui souhaitent mutualiser leurs publication qui sont déja sur un site WordPress existant, ceci permet en 5 minutes et sans travail supplémentaire de les partager dans une format interopérable.

Dans mon cas, ceci me permet d'éditer de récuperer des contenus en creative commons de mes sites existant et de les partager de manière automatique sur github et multibao où elles peuvent être consultées, copiées ou enrichies par d'autres sans nécessiter aucun travail supplémentaire de ma part.

## Comment synchroniser entre WordPress et Github ?

Pour synchroniser facilement des publications entre WordPress et Github, c'est ultra-simple: il vous faudra simplement installer deux plugin wordpress et leur donner un accès à votre compte github, le reste se fera automatiquement.

Pour cela

- sur votre site wordpress, identifiez vous et allez dans votre tableau de bord (vous devez être administrateur)
- allez dans Extensions > Ajouter 
- cherchez, installez puis activez l'extension WordPress GitHub Sync (https://wordpress.org/plugins/wp-github-sync/#description). Cette extension fera le travail de synchtonisation
- cherchez, installez puis activez l'extension WP-Markdown (https://wordpress.org/plugins/wp-markdown/). Cette extension permet l'écriture et l'import/export en format markdown.
- dans github, créer un repo où vous souhaitez. Pour cela cliquer sur le signe + en haut à gauche puis "New repository" (https://github.com/new). IMPORTANT: N'oubliez pas de cliquer sur "Initialize this repository with a README" pour que le repo soit utilisable directement.
- Revenez dans le tableau de bord WordPress et Allez dans Réglages > GiHub Sync

GitHub hostname



https://github.com/settings/tokens/new


## Pourquoi synchroniser entre WordPress et Github ?

A l'heure actuelle beaucoup de personnes publient des contenus sur leur site et WordPress est l'un des système de gestion de contenu les plus utilisés (20% du web environ tourne sous Wordpress).

Pourtant même si leurs auteur souhaitent partager leurs contenus/publications et les mettent en licence libre, en pratique ce partage n'est pas aisé, car le contenu n'est pas facilement reduplicable. 

Multibao part du principe que markdown, un format de formattage texte léger est un standard plus facile a utiliser que le HTML pour partager des contenus.
