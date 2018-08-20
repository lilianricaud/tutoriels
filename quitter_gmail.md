# Quitter Gmail

Gmail a été le plus difficile à quitter, non par difficulté technique mais pas confort. Utilisant gmail activement depuis 2005, je trouvai difficile d'avoir outil qui soit à la fois très fiable techniquement, rapide, avec une forte capacité de stockage, un bon antispam, une bonne ergonomie. J'étais accros à de petites fonctionnalités simples mais puissantes comme l'affichage des messages par conversations, la gestion de multiples adresses mail, l'annulation de l'envoi par erreur...

Même si depuis 2005 j'étais conscient de l'espionnage pratiqué par google (malgré tous leurs dires quand on voyait la qualité du ciblage des pubs dans ses mails on ne pouvait pas ignorer que gmail comprenait tout nos faits et gestes) et que adblock me protégeait des pubs, j'ai eu beaucoup de mal à partir.

Enfin cela été chose faite et j'utilise maitenant Thunderbird pour lire mes mails hébergés chez Ouvaton, hebergeur coopératif et éthique francophone.




## Processus de migration mail

- études des différentes alternatives à gmail en terme d'hebergement et d'interfaces
- choix d'un hebergeur: Ouvaton
- 


### Alternatives à gmail

### Migration de Gmail vers Zimbra
https://subfictional.com/2013/07/11/leaving-google-moving-email-and-calendar-to-zimbra/


Once my account was setup, the migration process was fairly straight-forward:

    Update MX records for my chosen domain.
    Start forwarding Gmail to new email addresses.
    Add Gmail address as external account in Zimbra via IMAP and start copying messages.
    Export main Google calendar and import into calendar called “Google” on Zimbra. Start copying relevant appointments to new main calendar.
    Begin the tedious process of updating email address everywhere.

### Utilisation du client Mail Cozy

Il est possible d'utiliser Cozy comme "client", c'est a dire un logiciel qui permet de lire et traiter les emails. Les emails eux mêmes viennent d'un serveur mail fourni par un hebergeur web ou google dans le cas de Gmail.

Le client de cozy permet d'aggreger les mails provenant de plusieurs serveurs mails (gmail, ouvaton)

En quelques clicks il est possible de configurer le client pour recevoir tous ses mails au même endroit. Il faut pour cela renseigner les paramètres suivant: imap et smtp.

Le client semble bien marcher, même si importer tous les mailx existants ne se fait tres bien.

Les etiquettes gmail, les conversations, tout est présent nativement

Bizarrement il ne semble pas possible d'envoyer de mail depuis Cozy :-/ verifier smtp (serveur d'envoi) ou support technique.

Paramètres ouvaton: https://ouvaton.coop/Les-bonnes-adresses
Paramètres Gmail: https://support.google.com/mail/troubleshooter/1668960?hl=fr-CA&rd=1


### Afterlogic webmail

Open source webmail proche d'une interface gmail avec intégration dans owncloud (expérimental). Note: il existe une version lite avec simplement la fonction webmail et une version pro payante avec agenda et contacts.

Installation:

Necessite téléchargement depuis le site:
http://www.afterlogic.org/webmail-lite

Puis installation par FTP dans dossier 

Activation via owncloud app manager

Indiquer l'URL ou le dossier est situé

### Zimbra Collaboration

Open source, fonctionnalité de conversations, filtres, antispam, etiquettes, 

Possède extensions (zimlets) qui enrichissent les fonctionnalités (undo sent, open pgp, intégration owncloud, ...)

Possibilité de migrer depuis serveur imap: 
https://wiki.zimbra.com/wiki/Mail_Migration
http://imapsync.lamiral.info/


### RainLoop

Webmail open source ressemblant beaucoup AfterLogic et préinstallé sur l'hebergeur coopératif Ouvaton.
Possède fonctionnalité conversations, étoiles/marquage, interface sobre, extensions.


