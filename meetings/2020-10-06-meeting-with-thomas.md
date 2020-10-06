Date: 2020-10-06

Participants:
* Thomas Beck 
* William Gathoye

## Business model

* Idée de business model additionnel:

    * Prendre inspiration sur les Amazon Dash qui permettaient (jadis) de
      mettre automatiquement dans le panier les produits pour lesquels notre
      stock personnel devenait faible.

    * L'idée ici est que des magasins (de préférence locaux) partenaires
      puissent automatiquement recommander à l'utilisateur des produits
      à acheter lorsque le produit de la même famille est concerné par une date
      de péremption limite.

    * Remplacement d'aliments considérés comme mal-bouffe par des alternatives
      locales et moins industrialisées.

    * Utilisation potentielle pas nécessairement par un B2C, mais un B2B comme
      un restaurateur ou une entreprise qui souhaiterait une simple gestion de
      stocks et pas nécessairement des denrées périssables.

## Idée d'implémentation

* On voit ça comme une application mobile avec un backend minimaliste.

* Niveau app mobile: Android avec Google Cloud Messaging (désormais nommé
  Firebase) avec gestion calendrier pour Android. 3 champs d'insertion (nom
  produit, descriptif et date de péremption).

* Peut-être pas le temps de gérer la session côté Android. On prévoit donc le
  renvoi d'un token à chaque requête.

* Peut-être l'ajout d'une photo voire d'une empreinte (digest) générée sur base
  du QR code et la matcher avec un dummy DB (bidonnage).

* Pour le backend, une communication toute simple en PHP avec échange JSON. Le
  stockage sera réalisé dans une DB MariaDB.

* Pour envoyer les push, une cron Linux qui s'exécutera tous les jours pour
  sélectionner les produits et prévenir la personne directement sur son mobile.

* Il ne serait pas possible d'utiliser un service tiers (à moins d'en trouver)
  qui permettraient une utilisation simplifiée de Firebase. Il existe Pushover
  (https://pushover.net/), mais ce service ne dipose pas d'un SDK Android. Le
  service Pushover permet juste d'être utilisé pour envoyer une notification
  push en fonction d'un événement. William utilise ce service pour être prévenu
  de la fin d'une tâche exécutée sur l'un de ses serveurs.


## Gestion du projet

Utilisation de la méthode SCRUM:

* On aura le temps de faire 2 livrables. Vu la taille du projet, on ne pourra
  diviser le projet qu'en 2 livrables: un en cours de route et le dernier pour
  la présentation YEP.

* Chaque X jours on fait un standup meeting (pas de taille à faire un standup
  meeting tous les jours).

* Peut-être prévoir un sprint review avec les parties prenantes (de préférence
  tous les 15 jours, ou en fonction de l'état d'avancement).
