# Caractéristiques de l'application :



#### Supports de l'application : 

- Mobile (Android et IOS)
- Web (application en ligne)



#### Fonctionnalités :

- Système de Login (Séparation entre compte professionnel et particulier) :
  - Écran classique de Login
  - Écran de création de compte
    - Lors de la première connexion, l'utilisateur peut alors choisir ses préférences alimentaires en ajoutant des tags à sa liste de préférences. l'idée est de pouvoir mieux le cibler ensuite lorsque des recettes lui seront proposées

- Liste de courses à faire :

  - Double liste : la première liste est la liste des catégories, la secondes est la liste des aliments et est imbriquée dans la première.
  - Les catégories et les aliments peuvent-être représentés par des émoticônes.
  - Les différents éléments de la liste sont associés à des "bulles" à cocher lorsque l'aliment considéré est acheté.
  - Une croix/icône de poubelle alignée à coté de l'aliment doit permettre de le supprimer de la liste de course.

- Écran de gestion d'un frigo virtuel :

  - Double liste catégories/aliments comme pour la liste de courses
  - Possibilité de "rechercher" un aliment par son nom ou son émoticône
  - Chaque aliment est associé à une date d'achat et une date de péremption
  - Une croix/icône de poubelle alignée à coté de l'aliment doit permettre de le supprimer du frigo virtuel.
  - Chaque aliment est associé à une liste de recette

- Système de scan de QR-code :

  - L'idée est de pouvoir scanner un QR-code au bas d'un ticket de caisse lorsque l'on fait nos courses afin de stocker l'ensemble des articles repris sur la facture dans le frigo virtuel.
  - La quantité d'informations que l'on peut stocker dans un QR-code excède rarement les 5000 caractères, donc en réalité le QR-Code cachera un URL vers un site web qui se chargera de récupérer les informations associées à cette facture et les insérera dans le frigo virtuel sur le compte de l'utilisateur.

- Système de notification des produits sur le point d'expirer :

  - Lorsqu'un aliment est sur le point de périmer, l'utilisateur reçoit alors une notification sur son téléphone lui permettant d'identifier le produit en question.
  - En plus de prévenir l'utilisateur de l'arrivée de la date limite d'un produit, l'utilisateur pourrait se voir proposer des recettes réalisables avec ce produit et d'autres produits déjà présents dans le frigo virtuel.

- Base de données :

  - Pour pouvoir déployer cette application, il faudrait mettre en place une base de données comportant l'ensemble des données relatives aux produits vendus en magasin.
  - La donnée essentielle à sauvegarder dans la base de données est la date de péremption du produit. C'est là le défi principale de l'application.

  



#### Structure de l'application :

- //A faire 



#### Style de l'application :

> Un style minimaliste (peu de boutons ou de fonctionnalités, pas trop surcharger le menu) et aux couleurs vivent rappelant fruits, légumes et la nature en générale doit être privilégié.



##### Écran de connexion :

![LoginScreen](../meetings/img/LoginScreen.png)

##### Écran de chargement :

![Loading-screen](../meetings/img/LoadingScreen.png)

##### Écran principal :

![MainScreen](../meetings/img/ListeCourse.png)

##### Scan d'un QR-code :

![QR-Code](../meetings/img/QRCode.png)



