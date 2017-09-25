# Fonctions utiles dans Gimp

Gimp est un logiciel puissant de retouche d'images. Voici quelques fonctions utiles.

## Faire apparaitre la boite à outils

Ctrl+B

## Rogner des images

- Sélectionner la zone à rogner
- Image > rogner selon la sélection

## Enregistrer l'image

pour avoir des images en jpg, choisir:
- Fichier > Exporter comme

Pour réenrgistrer une image déja en jpg, choisir:
- Fichier > Ecraser "nom de l'image"

## Gestion des calques

- Afficher la barre d'outils
- coller l'image
- dans la barre de gestion des calques choisir l'image appellée "sélection flottante", puis avec un clic droit choisir l'option "vers nouveau calque".

## Nettoyer une image scannée

Utiliser la fonction Couleurs > Luminosité-contraste 

en augmentant la luminosité et le contraste ont peut nettoyer un fond peu propre


## Redimensionner des images en lot avec Gimp

Installer d'abord le plugin DBP (David's Batch Processor)

http://members.ozemail.com.au/~hodsond/dbp.html

ou plus simple dans la logithèque Ubuntu installer le jeu de plugin "Dépôt d'extensions optionnelles pour GIMP"

Aller dans le menu suivant:

Filtres > Batch > Batch process

Il est possible de choisir les règles de transformation en lot

Choisir les images à modifier "input"

Choisir le menu "resize", choisir "keep ratio" pour garder les proportions

Choisir le format de sortie: "Output"

ATTENTION: par défaut, Gimp va remplacer les anciennes images par les nouvelles, veiller donc à conserver un copie des originales ailleurs au cas ou.

Pour changer cela, aller dans "rename"

Il est possible de choisir une répertoire d'entrée "source dir" et un répertoire de sortie "select dir"

Pour renomer avec prefixe ou postfixe: "Rename"

Quand tous les réglages ont été choisis, cliquer sur "Start" en bas à gauche de la fenètre.


## Source
CC-BY-SA
Lilian Ricaud 


