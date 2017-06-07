
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

### Configuration Github

Dans GitHub: 
-  créer un repo où vous souhaitez que les contenus soit synchronisés. Pour cela cliquer sur le signe + en haut à gauche puis "New repository" (https://github.com/new). IMPORTANT: N'oubliez pas de cliquer sur "Initialize this repository with a README" pour que le repo soit utilisable directement.
- générez un code "Oauth Token" à la page suivante: https://github.com/settings/tokens/new . Gardez ce code de coté, il vous sera demandé ensuite pour autoriser Wordpress à accéder à lire/écrire sur votre compte github. (Note: lors de la génération du code, j'ai coché toutes les options demandés pas sur que cela soit bon en terme de sécurité. a vérifier)

### Configuration WordPress

Sur votre site wordpress (vous devez disposee d'un site WordPress que vous gérez vous même et pas d'une instance WordPress.com):

-  identifiez vous et allez dans votre tableau de bord (vous devez être administrateur)
- allez dans Extensions > Ajouter 
- cherchez, installez puis activez l'extension WordPress GitHub Sync (https://wordpress.org/plugins/wp-github-sync/#description). Cette extension fera le travail de synchtonisation
- cherchez, installez puis activez l'extension WP-Markdown (https://wordpress.org/plugins/wp-markdown/). Cette extension permet l'écriture et l'import/export en format markdown.
- Allez dans Réglages > GiHub Sync. 

Dans la page réglages rentrez les infos suivantes: 

- GitHub hostname: laissez le contenus existant (https://api.github.com)
- Repository: le répo github avec lequels les contenus seront synchronisés/ L'adresse doit être du type: nom-utilisateur/nom-repo par exemple "lilianricaud/tutoriels"
- Oauth Token: copiez collez le code généré précédemment
- Webhook Secret: rentrez un mot de passe fort (pas sur de savoir à quoi il sert, mais il faut le faire).
- enregistrez les modifications.

### Exportez du contenu WordPress -> GitHub

Cliquer simplement sur "Export to GitHub". 

Le contenu publié sera disponible dans le repo github:

- https://github.com/nom_utilisateur/nom_repo

et lisible via MultiBAO à:

- http://www.multibao.org/nom_utilisateur/nom_repo

### Importez du contenu GitHub -> WordPress

Cliquer simplement sur "Import from GitHub"

Dans ce cas, le contenu du repo github choisi sera récupéré et publié dans WordPress.

### Cas où vous utilisez des custom post types

Si comme moi vous avez utilisé des custom post pour une raison quelquonque, l'exporteur ne fonctionnera pas.

Pour palier à cela, vous pouvez cependant convertir vos custom post en pages grace a l'excellent plugin Post-type switcher (https://wordpress.org/plugins/post-type-switcher/) avant de faire la manip d'export.

## Pourquoi synchroniser entre WordPress et Github ?

A l'heure actuelle beaucoup de personnes publient des contenus sur leur site et WordPress est l'un des système de gestion de contenu les plus utilisés (20% du web environ tourne sous Wordpress).

Pourtant même si leurs auteur souhaitent partager leurs contenus/publications et les mettent en licence libre, en pratique ce partage n'est pas aisé, car le contenu n'est pas facilement reduplicable. 

Multibao part du principe que markdown, un format de formattage texte léger est un standard plus facile a utiliser que le HTML pour partager des contenus.

## Source

- CC-BY-SA Lilian Ricaud
