___
#Bienvenue dans le README:
> ##Sur les concepts de Ruby on Rails
___

Sites Statiques:
*On entend par page statique, non pas une page sans mouvements ou sans animations, mais une page visible telle qu'elle a été conçue.
*Ces pages peuvent présenter toute forme de contenu, animations flash, images, musique, vidéo etc... mais elles sont toujours présentées de la même façon. Elles ne changent pas et c'est en ce sens qu'elles sont statiques.

Sites Dynamiques:
*En opposition aux pages statiques, les pages dynamiques permettent de présenter les informations de différentes manières selon l'interaction avec le visiteur. 
*Les pages sont alors construites "à la volée" grâce à une programmation conçue par le webmaster.
*Le contenu est issu d'une base de données en fonction de critères établis par l'internaute puis mis en page en temps réel. 
C'est le cas par exemple d'un site e-commerce: présentation des articles par thèmes, couleurs, prix etc... 
*C'est également le cas des blogs et des forums où les visiteurs peuvent participer au contenu du site. 
*C'est aussi le cas d'un système de mises à jour.


Les MVC:
Controller:
*Les contrôleurs effectuent le travail d'analyse des requêtes des utilisateurs, des soumissions de données, des cookies, des sessions et du «contenu du navigateur». Ils sont le gestionnaire aux cheveux pointus qui commande les employés autour.
*Le contrôleur renvoie le corps de la réponse (HTML, XML, etc.) et les métadonnées (en-têtes de mise en cache, redirections) au serveur. Le serveur combine les données brutes dans une réponse HTTP correcte et l'envoie à l'utilisateur.

Model:
Les modèles sont des classes Ruby. Ils parlent à la base de données, stockent et valident les données, exécutent la logique métier et font le gros du travail. Ils sont le gars potelé dans la salle arrière qui croque les chiffres.

View:
Les vues sont ce que l'utilisateur voit: HTML, CSS, XML, Javascript, JSON. Ils sont le représentant des ventes mettant en place des dépliants et des enquêtes de collecte, à la direction du gestionnaire. Les vues sont simplement des marionnettes lisant ce que le contrôleur leur donne. Ils ne savent pas ce qui se passe dans la pièce arrière.


Les routes:
Les routes permettent d’interpréter les URL et d’orienter vers les bonnes actions des controlleurs. La configuration se trouve dans le fichier config/routes.rb.


Les Base de Donnees:
Une base de données (database en anglais), permet de stocker et de retrouver l'intégralité de données brutes ou d'informations en rapport avec un thème ou une activité ; celles-ci peuvent être de natures différentes et plus ou moins reliées entre elles1,2. Dans la très grande majorité des cas, ces informations sont très structurées, et la base est localisée dans un même lieu et sur un même support. Ce dernier est généralement informatisé.


Get/Post:
*Get => C'est une méthode HTTP pour faire des requêtes sur Internet.

*Post => Une demande utilisant la méthode POST doit agir sur la collection de ressources; ajouter une nouvelle ressource à la collection


Le concept de Migration:
*Migrations are a convenient way for you to alter your database in a structured and organized manner. You could edit fragments of SQL by hand but you would then be responsible for telling other developers that they need to go and run them. You’d also have to keep track of which changes need to be run against the production machines next time you deploy.
*Active Record tracks which migrations have already been run so all you have to do is update your source and run rake db:migrate. Active Record will work out which migrations should be run. It will also update your db/schema.rb file to match the structure of your database.
*Migrations also allow you to describe these transformations using Ruby. The great thing about this is that (like most of Active Record’s functionality) it is database independent: you don’t need to worry about the precise syntax of CREATE TABLE any more than you worry about variations on SELECT * (you can drop down to raw SQL for database specific features). For example you could use SQLite3 in development, but MySQL in production

Les relations entre les models des BDD:
*Modèle	
Structure de données Intégrité des données Langage de définition de données Langage de requête
*Données	
Champ Table Vue Procédure stockée Déclencheur


Les fonctions du CRUD:
C(reate)R(ead)U(pdate)D(elete) désigne les quatre opérations de base pour la persistance des données, en particulier le stockage d'informations en base de données.
Plus généralement, il désigne les opérations permettant la gestion d'une collection d'éléments par une utilisation en front end.
Application dans les bases de données:

|Operation | SQL    | HTTP   |
|----------------------------|
|Create    | INSERT | POST   |
|Read      | UPDATE | GET    |
|Update    | UPDATE | PUT    |
|Delete    | DELETE | DELETE |
