# Développement d’un Système d’Authentification Sécurisé
L'authentification des utilisateurs en développement web est utilisée pour autoriser et restreindre l'accès des utilisateurs à certaines pages d'une application web.
*Système d'enregistrement*

# db.php– Connexion entre les Fichiers PHP et la Base de Données
Le fichier db.php est utilisé pour établir la connexion entre l'application PHP et la base de données MySQL. Il est inclus dans les autres fichiers pour centraliser la configuration de la connexion.


# hackathon.sql – Structure de la Base de Données
Le fichier hackathon.sql contient la structure de la base de données utilisée pour stocker les utilisateurs dans un tableau "users".


# register.php – Interface d'Enregistrement : Conception Intuitive et Sécurisée
![image](img/imgdev4.png)

Ce fichier permet à un nouvel utilisateur de s'inscrire via un formulaire comprenant : nom d'utilisateur, email, mot de passe et confirmation. Les données sont validées côté serveur et client.

# register.php – Validation et Sécurité : Prévention des Risques dès l'Inscription
![image](img/img.png)

En cas d'erreurs (format d’email invalide, mot de passe faible, confirmation erronée…), des messages clairs s’affichent pour guider l’utilisateur.

# login.php – Page de Connexion : Accès Sécurisé et Contrôle des Sessions 
![image](img/imgdev1.png)

Ce fichier vérifie les informations entrées par l’utilisateur en les comparant à celles de la base de données. En cas de correspondance, une session est créée. Sinon, un message d’erreur discret est affiché.

# dashboard.php – Accès Sécurisé au Tableau de Bord : Protection des Données Utilisateur
![image](img/imgdev3.png)

Une fois connecté, l'utilisateur est redirigé vers son tableau de bord personnel. Le fichier dashboard.php vérifie si une session valide existe, empêchant tout accès non autorisé.

# logout.php – Déconnexion Sécurisée de l’Utilisateur
Ce fichier permet à l’utilisateur de se déconnecter proprement. Il détruit la session active et redirige vers la page de connexion.

# Conclusion
Le projet repose sur des fichiers clairs et bien organisés (register.php, login.php, dashboard.php, logout.php), reliés à une base MySQL via db.php. Il offre une solution complète d’authentification avec des pratiques de sécurité robustes. Ce système constitue une base fiable pour tout site web nécessitant une gestion d’accès utilisateur.
