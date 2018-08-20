<!--

---
title: Migrer vers un serveur web éthique
description: J'utilisais depuis 10 ans Dreamhost un hebergeur américain qui marche très bien. Mais je voulais "rapprocher" mes données et entamer une démarche de maitrise du contenu. Voici la démarche.
image_url:
licence: CC-BY-SA 
---

-->

# Migrer vers un serveur web éthique

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






