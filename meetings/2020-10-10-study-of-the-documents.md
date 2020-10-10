![image-20201010172452868](C:\Users\Kouristoll\AppData\Roaming\Typora\typora-user-images\image-20201010172452868.png)

# Étude des documents fournis par les clients :



### Présentation du produit :

- Application mobile/web

- Envoie des notifications/rappels lorsqu'un produit est proche de la date limite de consommation : 

  > ​	"Ces notifications comprennent la date de péremptions du produit, son poids, ainsi qu’une recette qui permettrait à l’utilisateur d’utiliser l’aliment qui attend sa date limite de consommation"

- Une base de données sera disponible à l'avance, l'ajout de produit à cette base de données ne se fait pas via l'application.



### Utilisation :

1. Scan du ticket de caisse après avoir fait ses achats. (le ticket comporte un QR-Code)



### Interface de l'application :

- Page principale composée de deux messages : =="Scanner un ticket"== et =="Liste des aliments"==

- Lors d'un scan -> Un message de confirmation du bon fonctionnement de la procédure est affiché

- Lorsqu'on sélectionne "Liste des aliments" -> Affichage de tous les aliments achetés sous forme de liste

- Dans la liste => Afficher une photo "type" de chacun des produits

- Dans la liste => Affichage du poids de l'aliment

- >  "Le nom de l’aliment, son poids ainsi que sa date de péremption sont envoyés dans la notification" 



### Fonctionnalités demandées :

- Authentification de l'utilisateur -> Son compte est accessible sur diverses plateformes

- A la première utilisation -> demander les goûts de l'utilisateur afin de lui proposer des recettes plus adaptées à ses envies par la suite (recette belges, asiatiques, soupes, repas de fête, etc => ensemble de tags à sélectionner)

- Suppression d'un aliment de la liste

- Affichage des infos d'un aliment en le sélectionnant

- Chaque aliment est lié à une liste de recettes

- Gestion d'un frigo virtuel (on voit quel aliment on possède et ce qu'il nous manque -> moins de risques d'oublis)

- Scan de QR-Code (un seul scan pour récupérer toutes les infos -> Impossible techniquement parlant, les QR-Code sont trop limités et ne peuvent contenir autant d'informations)

- Base de donnée contenant l'ensemble des produits en magasin

- Les aliments ne doivent pas êtres encodés manuellement

  

##### idées de fonctionnalités de l'équipe informatique :

- Lien mise en avant des recettes qui peuvent êtres réalisée selon le poids du produit et des autres produits restant -> favoriser les aliments sur le point de périmer

- Onglet "recettes" pour poser des recettes avec l'aliment acheté.

- Onglets "mes aliments"

- Onglets promotions de grandes surfaces

  

