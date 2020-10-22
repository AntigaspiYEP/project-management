# Réunion YEP du Lundi 12 Octobre 2020 :

#### Personnes présentes :

- William Gathoye
- Thomas Beck
- Romain Van Geit
- Lise Laurent
- Gaël Baôo
- Belen Fernandes
- Drilon Ibraimi

#### Absences : N/A

#### Durée de la réunion : 1 heure 34 minutes

#### Objet : Premier meeting de compréhension de l’app.

#### Sujets abordés :

- L’aspect gamification est assez important, l’application soit elle-même drôle et ne pas être sérieux. Ne pas parler à la mode sérieux business comme les apps bancaires.

- Client imagine une app simple avec peu de fonctionnalités avec des couleurs flash qui rappellent les fruits et légumes sans gris et noir.

- Modifier le logo pour supprimer éventuellement ses couleurs trop sombres.

- Redhibitoire l’encodage manuel.

- Reprend le contenu du frigo mais pas uniquement, ça peut être conserves (dans la cave, etc.)

- Wish list: elle est encodée à la main, et il n’y a pas de lien entre la wish list et les produits réellement achetés. La wish list dans le futur pouraît être exploitée par les B2C pour savoir les intentiens réleles des acheteurs. Corrélation entre intentions et achats effectifs?
  Bulle/case à cocher.

- Base de données. C’est le plus gros challenge, il faut réussir à faire accepter aux grandes surface d’y stocker les dates de péremption sachant que le marché belge est déjà petit.

- Pas d’insertion de photo juste utilisation de l’appareil pour scanner le QR code. Lorsqu’on le scanne c’est un lien web qui s’ouvre dans le navigateur et là, l’app Android a un intent-filter sur l’URL pour l’ouvrir automatiquement; Et l’app récupère le contenu (bidon) renvoyé par le serveur: il populate directement une liste dans le frigo et n’écrase pas les données précédentes du frigo (il les fusionne). Il pourra toujours changer le lien dans le frigo.

- L’utilisateur devra toujours enlever manuellement les éléments du frigo. Certes l’aspect rédhibitoire de l’encodage n’est plus présent, mais il reste néanmoins cette étape similaire.

- Base de données bidon. On part de ce principe dans un monde idéal et une vision optimiste sur l’idée que se sera faisable dans un futur proche.

- 2 profils utilisateurs;

  - ménagère

  - B2B: restaurateur à choisir au moment de l’app. Seulement quand on sélectionne ce profil. Cette partie est payante et est accessible ultérieurement. Bidonnage pour la partie paiement.
    Gestion des stocks pour les restaurateurs c’est vraiment une plue-value commerciale. On ne développe pas du tout le B2B pour l’instant.

    → l’aspect restaurateur permet de se démarquer de la concurrence et des plateformes telles que To Good To Go.


  * Push:

    - l’alerte date de péremptions
      - liste des éléments futurs qui vont périmer				
      - Non développé : propose d’une vidéo d’une recette ? Comment faire ses frittes et un commerce où acheter les ingrédients.	
    - B2C: notifications en fonction des produits
      - pour plus tard: menu sain,
      - carte des magasins partenaires (Albinete, etc. Biologique, etc.)? Pas dans la première version. On reçoit une notif push en fonction de la localisation dans laquelle se trouve le commerce local qui dispose d’une offre pour l’utilisateur.
      - vente locale, valeur éco responsable et être au courant des promotions de ce vendeur.


    - l’owner (partnariat Loic fou de cuisine?, aspect gamification pour inciter la communauté,)

- B2B: payant pour des revenus mensuels (in app purchase)

- Le client marque son accord pour un développement Android. Une éventuelle implémentation pour iOS viendrait ultérieurement après le passage au YEP.

- Réunions les lundis à 17h30. Pour l’instant c’est toutes les semaines, par le futur ce sera peut-être tous les 15 jours pour coller à une idée plus développement agile (SCRUM). Fin du livrable le 15 décembre.

- Vidéo de présentation: attendre les mockups. C’est la partie cliente qui pourra se charger cette partie.

- Best effort, mais rappelons qu’il s’agit d’un prototype.

- Cette semaine leur fournir des wireframes. La partie technique pour réaliser les wireframes durant ce week-end le samedi 17.

- On leur donne accès pour samedi soir, ce qui leur laisse le dimanche pour y regarder et nous donner leur avis pour la réunion du lundi 17h30.

- Le dossier devra être adapté pour refléter les conditions belges. La CNIL n’ayant en effet autorité qu’en France, en Belgique, c’est la Commission de la Vie Privée. De même, l’article de loi est désormais remplacé par une implémentation locale du RGPD, une circulaire européenne.





