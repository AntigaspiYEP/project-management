#                             Présentation Anti-Gaspi



#### Personnes concernées :

- William Gathoye
- Thomas Beck
- Romain Van Geit



#### Introduction :

Avant de commencer à travailler sur l’application en elle-même, on a du réaliser des maquettes. Ceci s’est fait en 2 étapes : d’abbord les wireframes et ensuite les mockups.

Les wireframes: qui sont la conception de l'interface sans couleur, souvent réalisé à la main. Étape dédiée à savoir où vont être placés les éléments.

Les mockups: qui sont une représentation visuelle quasiment au pixel prêt de ce que sera le visuel de l'application. Donc qui représente l'interface le plus fidèlement possible à ses wireframes.

Ensuite, après la validation de ceux-ci par le client, on a pu commencer à développer l’application sur bases des des mockups présentés.



#### Technologies utilisées :

Pour les mockups et les wireframes, on avait le choix entre 3 applications : Sketch,Invision et Marvel.

Sketch étant payant et réserver à macOS, il a directement été éliminé. Invision, une application web qui dispose d’une version gratuite, beaucoup moins complète et Marvel, celle qui a été choisie, une alternative à Invision et aussi souvent utilisée en entreprise.

Concernant l’application en elle-même, le projet du client étant une application mobile, on avait pas énormément de choix. On pouvait la réaliser pour Ios ou pour Android. On a donc décidé de la réaliser en Android, le marché étant composé actuellement de 80% de téléphones android et 19% d’Iphones. De plus c’est une technologie qu’on était en train d’apprendre dans le cadre d’un autre cours, cela nous permettait d’avoir un temps de formation plus court et de commencer le projet le plus vite possible.



#### L'application :

- Login :

  Pour commencer, quand l’application est lancée on arrive sur une page qui nous propose de se connecter grâce à ce formulaire.

  ![image-20201206214010482](C:\Users\vange\AppData\Roaming\Typora\typora-user-images\image-20201206214010482.png)

  

  

- Frigo virtuel :

  Si l’utilisateur a déjà un compte il peut directement remplir le formulaire pour accéder à l’application, si il n’en possède pas il peut en créer un. Une fois connecté, on arrive sur la page principale de l’application.

  ![image-20201206214208442](C:\Users\vange\AppData\Roaming\Typora\typora-user-images\image-20201206214208442.png)

  

  Sur cette page on peut voir directement qu’on reçoit une notification pour nous prévenir qu’un aliment arrive bientôt à sa date de péremption. On peut aussi voir dans le menu en bas de l’écran la petite pastille rouge qui nous indique le nombre d’aliments périmés dans le frigo. Ensuite on peut constater à droite de l’image du frigo, le nombre total d’aliments que le frigo possède, ainsi que le nombre d’aliments qui périment bientôt et les aliments qui le sont déjà.

  

- Qr-code :

  Dans le menu en bas de l’écran, le logo du milieu nous permet d’arriver sur l’écran qui nous permet de scanner un QR code. 

  

![image-20201206214350189](C:\Users\vange\AppData\Roaming\Typora\typora-user-images\image-20201206214350189.png)

Une fois le QR code scanné, c’est un lien web qui s’ouvre dans le navigateur et là, l’app Android a un intent-filter sur l’URL pour l’ouvrir automatiquement. Et l’app récupère le contenu (bidon) renvoyé par le serveur. Il rempli directement une liste dans le frigo et la fusionne avec les données déjà présentent.



- Liste de course :

  L’avant dernier logo en bas de l’écran nous permet d’accéder à une liste de course…

  ![image-20201206214515339](C:\Users\vange\AppData\Roaming\Typora\typora-user-images\image-20201206214515339.png)

  Une fois arrivé sur cette page, l’utilisateur a la possibilité d’ajouter des nouveaux articles à sa liste de course en cliquant sur le bouton « + » en bas à droite de l’écran. Il a aussi la possibilité de modifier un article en faisant glissé son doigt vers la droite sur l’article qu’il veut modifier. Il a aussi possibilité de supprimer un élément en faisant la même chose mais en faisant glissé son doigt vers la gauche cette fois-ci.

  

- Options :

  //A finir



#### Méthodologie de travail :

On a décidé d'utiliser la méthode agile SCRUM, ce qui nous permettait d'avoir une approche plus pragmatique des besoins du client en autorisant une	  réactivité permanente à ses demandes et aux besoins évolutifs des utilisateurs, ce qui nous permettait de privilégier la réalisation d'un produit opérationnel, dans un délai contraint.  Cette méthode agile est aussi avantageuse dans le sens où le client ne doit pas attendre la toute fin du projet pour avoir une impression de ce que donne son projet.

Pour cela, on s'est mit d'accord pour faire des réunions avec les clients toutes les 1-2 semaines le lundi soir en fonction de ce qu'on avait à leur présenter.  On fournit des livrables rapidement au client de façon pour lui à nous faire ses retours tôt dans le processus de création, nous permettant ainsi d'ajuster le tir si la direction prise par le développement est incorrecte ou si en cours de route, on se rend compte que le business model ne tient pas et nécessite des ajustements.

