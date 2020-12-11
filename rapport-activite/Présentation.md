#                             Présentation Anti-Gaspi



#### Personnes concernées :

- William Gathoye
- Thomas Beck
- Romain Van Geit



## Présentation du projet

Nous avons décidé de travailler sur le projet Anti-Gaspi, le but de cette application étant d’éviter le gaspillage alimentaire en envoyant des rappels sur l’écran de l’utilisateur de l’application lorsque les aliments sont presque périmés afin d’aider l’utilisateur à consommer le produit avant qu’il soit périmé. L’objectif de ce produit est donc d’aider le consommateur à diminuer son gaspillage alimentaire. L'application est également utile lorsque l’utilisateur fait ses courses, il sait se connecter sur son compte afin de regarder quel aliment il lui reste dans son frigo et quel aliment il lui manque. Le consommateur a donc moins de risque d’oublier quelque chose lorsqu’il fait ses courses.

Le fonctionnement de l’application est très simple : il suffit de scanner un « QR code » se trouvant sur les articles que vous voulez ajouter à votre frigo grâce à la caméra de votre appareil ( téléphone portable ou tablette ). Lorsque élément est scanné, il sera ajouté au frigo virtuel. On a aussi la possibilité de créer une « Liste des aliments », une liste de tous les aliments achetés est disponible. Il est possible de supprimer les produits s’ils ont déjà été utilisés. 



## L'application :

- **Login :**

  Pour commencer, quand l’application est lancée on arrive sur une page qui nous propose de se connecter grâce à ce formulaire.

  ![image-20201206214010482](C:\Users\vange\AppData\Roaming\Typora\typora-user-images\image-20201206214010482.png)

  

  

- **Frigo virtuel :**

  Si l’utilisateur a déjà un compte il peut directement remplir le formulaire pour accéder à l’application, si il n’en possède pas il peut en créer un. Une fois connecté, on arrive sur la page principale de l’application.

  ![image-20201206214208442](C:\Users\vange\AppData\Roaming\Typora\typora-user-images\image-20201206214208442.png)

  

  Sur cette page on peut voir directement qu’on reçoit une notification pour nous prévenir qu’un aliment arrive bientôt à sa date de péremption. On peut aussi voir dans le menu en bas de l’écran la petite pastille rouge qui nous indique le nombre d’aliments périmés dans le frigo. Ensuite on peut constater à droite de l’image du frigo, le nombre total d’aliments que le frigo possède, ainsi que le nombre d’aliments qui périment bientôt et les aliments qui le sont déjà.

  

- **Qr-code :**

  Dans le menu en bas de l’écran, le logo du milieu nous permet d’arriver sur l’écran qui nous permet de scanner un QR code. 

  

![image-20201206214350189](C:\Users\vange\AppData\Roaming\Typora\typora-user-images\image-20201206214350189.png)

Une fois le QR code scanné, c’est un lien web qui s’ouvre dans le navigateur et là, l’app Android a un intent-filter sur l’URL pour l’ouvrir automatiquement. Et l’app récupère le contenu (bidon) renvoyé par le serveur. Il rempli directement une liste dans le frigo et la fusionne avec les données déjà présentent.



- **Liste de course :**

  L’avant dernier logo en bas de l’écran nous permet d’accéder à une liste de course…

  ![image-20201206214515339](C:\Users\vange\AppData\Roaming\Typora\typora-user-images\image-20201206214515339.png)

  Une fois arrivé sur cette page, l’utilisateur a la possibilité d’ajouter des nouveaux articles à sa liste de course en cliquant sur le bouton « + » en bas à droite de l’écran. Il a aussi la possibilité de modifier un article en faisant glissé son doigt vers la droite sur l’article qu’il veut modifier. Il a aussi possibilité de supprimer un élément en faisant la même chose mais en faisant glissé son doigt vers la gauche cette fois-ci.

  

- **Options :**

  //A finir



## Méthodologie de travail :

On a décidé d'utiliser la méthode agile SCRUM, ce qui nous permettait d'avoir une approche plus pragmatique des besoins du client en autorisant une	  réactivité permanente à ses demandes et aux besoins évolutifs des utilisateurs, ce qui nous permettait de privilégier la réalisation d'un produit opérationnel, dans un délai contraint.  Cette méthode agile est aussi avantageuse dans le sens où le client ne doit pas attendre la toute fin du projet pour avoir une impression de ce que donne son projet.

Pour cela, on s'est mit d'accord pour faire des réunions avec les clients toutes les 1-2 semaines le lundi soir en fonction de ce qu'on avait à leur présenter.  On fournit des livrables rapidement au client de façon pour lui à nous faire ses retours tôt dans le processus de création, nous permettant ainsi d'ajuster le tir si la direction prise par le développement est incorrecte ou si en cours de route, on se rend compte que le business model ne tient pas et nécessite des ajustements.

Au niveau de la répartition des tâches, on a essayé de se répartir les tâches au maximum. Etant compliqué de coder à 3 en même temps sur l'application, William et Thomas, étant plus à l'aise avec l'Android, se sont chargés de la conception de l'application en se partageant différentes fonctionnalités. Romain s'est alors chargés de tout ce qui était documents de gestion. 

Afin d'avoir une vision globale sur le projet et que tout le monde puisse être mit au courant des nouvelles fonctionnalités intégrées et des nouveaux documents importés, on a décidé d'utiliser la plateforme GitHub sur laquelle on a créé une organisation Anti Gaspi qui contient 2 repositories : Android-app ( pour l'application en elle-même ) et Project-management pour tout ce qui est documents externes.



## Estimation du planning :

Pour cette partie, on a d'abord réalisé un diagramme de PERT reprenant les différentes tâches à réaliser sur le projet en calculant les dates au plus tôt, au plus tard ainsi que les différentes marges.

 

![Yep-PERT-Diagram](C:\Users\vange\Documents\COURS\Labo\Anti-Gaspi\project-management\management-documents\Yep-PERT-Diagram.png)



Sur base de ce diagramme de PERT ci-dessus, on a pu alors réaliser le diagramme de Gantt que vous retrouvez ci-dessous. Sur ce diagramme on peut apercevoir l'enchainement des différentes parties de la réalisation du projet à partir du 6 octobre jusqu'à la finalisation du livrable, le 15 décembre. 

<img src="C:\Users\vange\AppData\Roaming\Typora\typora-user-images\image-20201211151128292.png" alt="image-20201211151128292" style="zoom: 200%;" />



## Choix technologiques :

- ### Evolution du développement :

  Avant de commencer à travailler sur l’application en elle-même, on a du réaliser des maquettes. Ceci s’est fait en 2 étapes : d’abbord les wireframes et ensuite les mockups.

  Les wireframes: qui sont la conception de l'interface sans couleur, souvent réalisé à la main. Étape dédiée à savoir où vont être placés les éléments.

  Les mockups: qui sont une représentation visuelle quasiment au pixel prêt de ce que sera le visuel de l'application. Donc qui représente l'interface le plus fidèlement possible à ses wireframes.

  Ensuite, après la validation de ceux-ci par le client, on a pu commencer à développer l’application sur bases des des mockups présentés.

  

- ### Technologies utilisées

  Pour les mockups et les wireframes, on avait le choix entre 3 applications : Sketch,Invision et Marvel.

  Sketch étant payant et réserver à macOS, il a directement été éliminé. Invision, une application web qui dispose d’une version gratuite, beaucoup moins complète et Marvel, celle qui a été choisie, une alternative à Invision et aussi souvent utilisée en entreprise.

  Concernant l’application en elle-même, le projet du client étant une application mobile, on avait pas énormément de choix. On pouvait la réaliser pour Ios ou pour Android. On a donc décidé de la réaliser en Android, le marché étant composé actuellement de 80% de téléphones android et 19% d’Iphones. De plus c’est une technologie qu’on était en train d’apprendre dans le cadre d’un autre cours, cela nous permettait d’avoir un temps de formation plus court et de commencer le projet le plus vite possible.



## Conclusion

Nous avons vraiment aimé travailler sur ce projet. Premièrement, c'était une expérience intéressante nous permettant de travailler et donc collaborer avec des clients, ceci nous a apprit à communiquer avec eux. On a pu aussi voir que les idées du client au départ et ce qui est réellement faisable dans une application sont différentes. Cet exercice nous a aussi permit d'appliquer les méthodes de gestion de projet vues en classe, qu'on avait pas eu l'occasion d'appliquer réellement jusqu'à maintenant. Nous pensons que c'est une bonne chose pour notre insertion dans le monde professionnel.

Deuxièmement, les contraintes rencontrées ont surtout été au niveau de la répartition du travail,de la gestion de la charge de travail et de la coordination. Aillant pas mal d'autres projets à côté, on ne pouvait pas se consacrer à temps plein sur celui-ci et chacun d'entre nous avions un planning différent. On a aussi rencontrés quelques difficultés au niveau du design de l'application car notre équipe ne possédait malheureusement pas d'infographistes pour gérer cette partie. 

Enfin, nous sommes satisfaits de notre participation au projet "Anti-Gaspi" puisque nous avons atteint les objectifs voulus et demandés par les clients.