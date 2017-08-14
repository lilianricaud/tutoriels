# Insérer des images en lot dans un fichier mardown

Pour intégrer une images dans un fichier mardown il faut utiliser un code.

> "![](nom_de_l_image.extension)"

Pour insérer une images, ce travail est simple, mais dès qu'il y plusieurs images, c'est très fastidieux.

Pour éviter de taper de manière fastidieuse ce code, il est possible d'utiliser une série de manipulation et de raccourcis clavier afin de rajouter ce code autour du nom des images pour des dizaines ou des centaines d'images, et ce, sans effort supplémentaire.

ATTENTION: avant de démarrer, assurez vous que les images soient bien nommées:
- pas de majuscules (sources d'erreur)
- pas d'espace (utilisez underscore_)
- pas de caractères spéciaux (accents, ...)

vous éviterez ainsi des bugs inutiles.

## Procédure

1. Dans votre dossier contenant les images, sélectionner toutes les images (Ctrl+A)
2. dans un fichier texte Gedit, coller les noms de fichier (Ctrl+V)
Vous obtenez un lien du style "/home/lilian/SparkleShare/patterning-complexity/images/DesignProcessContinuum.png"
3. Dans Gedit sélectionnez la partie à éliminer ici "/home/lilian/SparkleShare/patterning-complexity/" et copier la (Ctrl+C)
4. Utiliser la fonction remplacer (Ctrl+H) et coller le texte à éliminer puis ajouter la première partie du code markdown d'intégration des images "![](" 
5. sélectionner la fin des images ici ".jpg", copier (Ctrl+C), et appeler la fonction remplacement (Ctrl+H), coller le contenu (Ctrl+V), puis dans la zone det texe a ajouter, mettez ".jpg)" pour que la parenthèse de colture soit ajoutée à la fin de toutes les images.
6. il ne reste ensuite plus qu'a insérer ces codes dans le fichier .md


## Source
CC-BY-SA
Lilian Ricaud 


