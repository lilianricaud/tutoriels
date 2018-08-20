
# Degooglization

Au cours des dernières années j'ai réduit l'usage des outils google big brother devenu bien trop puissant, voici comment: 

## Google Search -> DuckDuckGo

J'ai très facilement quitté la recherche google depuis les révélation des Snowden et je suis passé sur DuckDuckGo qui ne trace pas ses usagers.

Même si la recherche est legerement moins performante pour les sites en français, l'outil marche très bien. Depuis 2013, DuckDuckGo est mon moteur par défaut et je ne suis jamais revenu en arrière.

Je continu à utiliser onctuellement google pour des recherches speicfiques, quand DuckDuckGo ne suffit pas (en français par exemple ou pour les images).

Dans ce cas, j'utilise les recherches bang!

g! + mots clés = recherche directe dans google
gi! + mots clés = recherche directe dans google images (pratique pour trouver des images en creative commons)



## Google Slides -> Markdown presentation

Le logiciel de bureau Marp premet de créer tre ssimplement des presentations au format markdown. Les contenus sont donc plus facilement interopérables avec d'autres outils.

Même si les présentations ont une limite de complexité, elle suffisent pour des diapos basiques (titre, image de fond, liste à puce, ...)

en utilisant les commentaires markdown, il est même possible de rajouter dans le contenu de la prez des notes de présentateurs, ainsi la même fiche peut servir en format présentation ou texte plus complet.

## Google texte -> pad, hackmd

les pads sont moins puissants, mais facile à créer, possèdes fonctions d'accès privés.

les hackmd ressemblent aux hackpad, mais utilisent markdown.




### Alternatives à gmail

### GMail: Migration mail depuis google

Nouveau serveur mail
Couplage avec afterlogic sur owncloud ?

Migration de Gmail vers Zimbra
https://subfictional.com/2013/07/11/leaving-google-moving-email-and-calendar-to-zimbra/

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


## Processus de migration mail

Once my account was setup, the migration process was fairly straight-forward:

    Update MX records for my chosen domain.
    Start forwarding Gmail to new email addresses.
    Add Gmail address as external account in Zimbra via IMAP and start copying messages.
    Export main Google calendar and import into calendar called “Google” on Zimbra. Start copying relevant appointments to new main calendar.
    Begin the tedious process of updating email address everywhere.

I had a couple of choices when migrating all of my email messages:

