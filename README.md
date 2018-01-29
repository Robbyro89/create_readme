___
___

# Bienvenue dans le **README** :
## sur des concept de Ruby on Rails.
___
___

##### Site Statiques Vs Sites Dynamiques:

###### 1. Sites Statiques:
* On entend par page statique, non pas une page sans mouvements ou sans animations, mais une page visible telle qu'elle a été conçue.
* Ces pages peuvent présenter toute forme de contenu, animations flash, images, musique, vidéo etc... mais elles sont toujours présentées de la même façon. Elles ne changent pas et c'est en ce sens qu'elles sont statiques.

###### 1. Sites Dynamiques:
* En opposition aux pages statiques, les pages dynamiques permettent de présenter les informations de différentes manières selon l'interaction avec le visiteur. 
* Les pages sont alors construites "à la volée" grâce à une programmation conçue par le webmaster.
* Le contenu est issu d'une base de données en fonction de critères établis par l'internaute puis mis en page en temps réel. 
C'est le cas par exemple d'un site e-commerce: présentation des articles par thèmes, couleurs, prix etc... 
* C'est également le cas des blogs et des forums où les visiteurs peuvent participer au contenu du site. 
* C'est aussi le cas d'un système de mises à jour.
___

##### Les MVC:

###### 1. Controller:
* Les contrôleurs effectuent le travail d'analyse des requêtes des utilisateurs, des soumissions de données, des cookies, des sessions et du «contenu du navigateur». Ils sont le gestionnaire aux cheveux pointus qui commande les employés autour.
* Le contrôleur renvoie le corps de la réponse (HTML, XML, etc.) et les métadonnées (en-têtes de mise en cache, redirections) au serveur. Le serveur combine les données brutes dans une réponse HTTP correcte et l'envoie à l'utilisateur.

###### 1. Model:
Les modèles sont des classes Ruby. Ils parlent à la base de données, stockent et valident les données, exécutent la logique métier et font le gros du travail. Ils sont le gars potelé dans la salle arrière qui croque les chiffres.

###### 1. View:
Les vues sont ce que l'utilisateur voit: HTML, CSS, XML, Javascript, JSON. Ils sont le représentant des ventes mettant en place des dépliants et des enquêtes de collecte, à la direction du gestionnaire. Les vues sont simplement des marionnettes lisant ce que le contrôleur leur donne. Ils ne savent pas ce qui se passe dans la pièce arrière.

###### 1. Vue d'ensemble du fonctionnement de la **MVC**:
à l'aide du schéma suivant:

![Schéma MVC](/home/user/Images/mvc_schematic.png)
___

##### Les routes:
  Les routes permettent d’interpréter les URL et d’orienter vers les bonnes actions des controlleurs. La configuration se trouve dans le fichier config/routes.rb.
___

##### Les Base de Donnees:
  Une base de données (database en anglais), permet de stocker et de retrouver l'intégralité de données brutes ou d'informations en rapport avec un thème ou une activité ; celles-ci peuvent être de natures différentes et plus ou moins reliées entre elles1,2. Dans la très grande majorité des cas, ces informations sont très structurées, et la base est localisée dans un même lieu et sur un même support. Ce dernier est généralement informatisé.
___

##### Get Vs Post:

###### 1. Get:
  C'est une méthode HTTP pour faire des requêtes sur Internet.

###### 1. Post:
  Une demande utilisant la méthode POST doit agir sur la collection de ressources; ajouter une nouvelle ressource à la collection
___

##### Le concept de Migration:
* Les migrations sont un moyen pratique de modifier votre base de données de manière structurée et organisée. Vous pouvez éditer des fragments de SQL à la main, mais vous devrez alors indiquer aux autres développeurs qu'ils doivent les exécuter. Vous devez également garder la trace des modifications qui doivent être exécutées sur les machines de production la prochaine fois que vous déployez.
* Active Record trace les migrations qui ont déjà été exécutées. Il vous suffit de mettre à jour votre source et d'exécuter rake db: migrate. Active Record déterminera quelles migrations doivent être exécutées. Il mettra également à jour votre fichier db / schema.rb pour qu'il corresponde à la structure de votre base de données.
* Les migrations vous permettent également de décrire ces transformations en utilisant Ruby. Ce qui est génial, c'est que (comme la plupart des fonctionnalités d'Active Record), il est indépendant de la base de données: vous n'avez pas besoin de vous préoccuper de la syntaxe précise de *create table*, pas plus que vous ne craignez les variations sur *select*. SQL pour les fonctionnalités spécifiques à la base de données). Par exemple vous pourriez utiliser SQLite3 en développement, mais MySQL en production
___

##### Les relations entre les models des BDD:
* Modèle	
Structure de données Intégrité des données Langage de définition de données Langage de requête
* Données	
Champ Table Vue Procédure stockée Déclencheur
___

##### Les fonctions du CRUD:
* **C**(reate) **R**(ead) **U**(pdate) **D**(elete) désigne les quatre opérations de base pour la persistance des données, en particulier le stockage d'informations en base de données.
* Plus généralement, il désigne les opérations permettant la gestion d'une collection d'éléments par une utilisation en front end.
* Application dans les bases de données (tableau ci-dessous):

| Operation | SQL    | HTTP   |
| --------- | ------ | ------ |
| Create    | INSERT | POST   |
| Read      | UPDATE | GET    |
| Update    | UPDATE | PUT    |
| Delete    | DELETE | DELETE |
