# Meeting technique du 2020-11-02

Date: 2020-11-03

Heure: 20h00

Durée: 04h00

Présents:

- William Gathoye
- Thomas Beck
- Romain Van Geit

## Sujets

* Thomas: Le projet semble stagner, on va devoir accélérer le travail au niveau
  du dev, travailler quelques heures par semaine ne suffit plus. Il faut faire
  ça quasiment de façon quotidienne histoire de présenter quelque chose au
  client au plus vite et respecter notre approche Agile.
    * William: OK pour les jours soir à 20h00 jusqu'au 9 novembre, on
      envisagera une rédaptation du rythme par la suite.

* Thomas: Un prototypage est OK, pas besoin nécessairement d'une app
  fonctionnelle. Les projets concurrents semblent utiliser 2 outils permettant
  un prototypage plus aisé:
    * [GlideApps](https://www.glideapps.com) permettant d'utiliser un template
      d'application et de se greffer à une feuille de calcul Google
      Spreadsheets.
        * William: On est cantonné à une liste de templates bien définie. Au
          niveau des data, on est limité à une simple feuille de calcul, pas
          possible d'avoir des données métiers complexes. De même, on remarque
          l'absence d'un système de double liste dans les templates et [aucun
          module de scan de QR
          code](https://www.glideapps.com/templates?category=All) ne semble
          présent.
        * Romain: Après une fouille plus approfondie, il serait peut-être
          possible, mais ces modules sont payants. Et on ne sait s'en assurer
          qu'après avoir payé.
            * William et Thomas: No go.

    * Thomas: Utiliser un outil nommé Figma. Il suffit de regarder une [vidéo
      d'introduction](https://www.youtube.com/watch?v=3q3FV65ZrUs&ab_channel=DesignCourse)
      pour prendre l'outil en mains.
        * William: Ne comprend pas bien ce que ce nouveau système apporte par
          rapport aux 2 Marvel déjà existants. La learning curse de Figma semble
          impressionante, rien que faire l'ajout d'un template prend un temps
          fou là où sur Marvel en 5 secondes, on peut déjà ajouter [démo].
        * Thomas: Nécessite alors 2 comptes.
        * William: Pas un souci, c'était de toutes façon prévu, on continue sur
          cette voie, et en concervant 2 comptes dédiés: un pour les wireframes
          et un pour les mockups.
            * Romain: Quand on se connecte, les autres sessions sont
              déconnectées.
            * William: Certes sur la conception ça poserait souci, mais on est
              à la fin des wireframes, reste plus qu'à faire les mockups et
              après on ne s'en sert plus. La conversion des wireframes en
              mockups ne nécessite pas d'être plusieurs dessus. Marvel fournit
              un lien de partage (un prototype animé) permettant une
              consultation à plusieurs. On a déjà fourni le lien de la première
              version des wireframes au client.
                * Thomas: OK dans ce cas.

    * William: On partirait alors dans ce cas comme on avait prévu
      initiallement, une simple app de démo Android réalisée via le designer
      d'Android Studio avec des intents fonctionnels.
        * Thomas: OK, mais dans ce cas, on va devoir passer à coté de la partie
          serveur, threads d'app etc. sinon pas le temps et utiliser des
          données hardcodées.
        * William: Dommage qu'on ait les autres cours :(
    
* Recherche de designs existants et d'UI qu'on pourrait déjà importer
  directement en XML.
    * Romain: Tous les bons produits qu'on trouve sont payants ou ne tournent
      pas.
    * William: Réussite à trouver quelques sites, les seuls modèles trouvés
      datant de 2018 nécessitent de mettre à jour les instructions de build
      gradle.
        * William: Ok, quand on se remet dans le bain pas si difficile. Les
          modèles ne sont toutefois pas exploitables tels quels mais donnent
          une idée comment agencer le code XML pour avoir une interface
          agréable.
        * William: La plupart des designs utilisent un simple nested layout
          avec comme parent un layout vide disposant d'une image
          d'arrière-plan. Utiliser une image d'illustration d'arrière plan
          permet de rendre le truc plus pro. [Merci
          Icons8](https://icons8.com/illustrations/kitchen%20set)
        * William: Les devs de Google fournissent des [sample de code desquels
          s'inspirer](https://developer.android.com/samples).

    * William: On tombe souvent sur [ce site ](https://wsdesign.in) mais
      l'iscription ne fonctionne pas. Heureusement, quand on cherche un peu on
      tombe sur les [sources GitHub](https://github.com/wsdesignuiux).
      Attention, le projet d'app se trouve toujours dans le sous dossier `app`.
      Donc quand on l'ouvre avec Android Studio il faut bien aller dans le souc
      dossier même si le dossier parent est correctement identifié comme projet
      Android par Android Studio.

    * William: Dribble est également une bonne source d'inspiration (nécessite
      un compte pour ouvrir les liens et télécharger les projets Android Studio
      sur un site tiers).
      [src.](https://dribbble.com/wsdesignuiux/projects/512122-WSDesign)
      [src.](https://dribbble.com/shots/6197569-Free-android-login-designs-with-xml-source-code)

    * William: [WorldOfUiUX](https://www.worldofuiux.com) fonctionne et donne
      des templates Android Studio.

    * Thomas: Lire un peu sur [Material
      Design](https://material.io/resources/get-started#design) serait bien.

    * William: [La lecture du blog officiel des devs
      Android](https://android-developers.googleblog.com) permet de trier et
      voir si certains articles qu'on trouverait en ligne sont encore valides
      ou pas (Android bouge beaucoup).


* Standardisons nous sur les versions employées:

    * VSD: Android Pixel 3a, 4096 Mio de RAM
    * API 30 (Android R)
    * Dans `build.gradle` (version `Module` **pas** `Project`), s'assurer que
      les variables suivantes soient définies comme suit:
        * `compileSdkVersion 30`
        * `buildToolsVersion "30.0.2"`
        * `minSdkVersion 25`
        * `targetSdkVersion 30`
    * On s'assurera donc d'avoir dans le SDK Manager d'Android d'avoir installé
      les API pour la version 25 (Android 7.1.1) et la version 30 (Android 11)
    * S'assurer également d'avoir l'accélérateur Intel installalé.

* Romain: Espace disque insuffisant.
    * Désinstallation complète d'Android Studio et SDK
    * Nettoyage de Windows 10
    * Réinstallation sur disque dur bénéficiant de plus de place
    * Débugging du souci: `Waiting for target to come online`.
        * Un `Wipe Data` ou un `Cold boot` ne servaient à rien
        * `adb kill-server`, activer Les `Developers Options`en cliquant 7 fois
          sur `Build number` dans les options d'Android sur l'AVD, et essayer
          de cliquer sur la boite de dialogue `Authorize USB debugging` a résolu
          le souci. Il semblerait qu'on ait affaire à [une race condition
          ici](https://stackoverflow.com/questions/42816127/waiting-for-target-device-to-come-online#comment114332387_43187806)
          entre l'emulateur et Android Studio qui simule la pression du bouton
          autoriser.

