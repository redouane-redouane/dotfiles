########################    Logiciels à installer   ########################

- WAMP server
- neo4j desktop:
    connexion entre php et neo4j:
        - installer composer
        - suivre les insructions du lien: https://github.com/graphaware/neo4j-php-client
        - copier le dossier vendor créé dans le dossier PFE/Application/traitement
- python:
    Bibliothèques python: flask, numpy, pandas, pulp, py2neo
- docker:
    installer le server openmaptiles: suivre les instructions du lien: https://openmaptiles.com/server/#install selon le système d'exploitation

########################    Utilisation     ########################

- Créer une base de données neo4j vide

- Remplir la base de données orientée graphe neo4j, avec les scripts qui se trouvent dans le dossier DB_LMTO dans l'ordre suivant:
    - nodes.
    - edges.
    - security.
    - distance.

    Copier à chaque fois tout le contenu d'un fichier puis le coller dans le champs des requêtes.

- Créer les noeuds des utilisateurs de l'application dans la base de données avec des requêtes de type:
    CREATE (n:User{ID_User:1, username:'admin', password:'admin'})

- Lancer le serveur de cartes avec docker
    accéder au lien du serveur de cartes local pour récupérer les adresses des cartes pour les remplacer dans le code javascript qui fait appel à ce serveur

- Lancer le serveur de calcul qui se trouve dans le chemin PFE/Calcule_path.py

- Mettre le dossier PFE dans le répértoire wamp/www

- Lancer WAMP server

- Accéder l'adresse:
    localhost/PFE/Application/login.php
    introduire les identifiants des utilisateurs insérés précédemment
