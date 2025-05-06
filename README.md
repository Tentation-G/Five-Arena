📘 FiveArena – Documentation d'installation et d'utilisation | 5arena-mvc
🧾 Présentation

FiveArena est une application web développée en PHP avec une architecture MVC.
Elle permet de gérer la réservation de terrains de sport (ajout, édition, suppression), la gestion des utilisateurs et des réservations via un back-office.


🛠️ Prérequis
  PHP ≥ 7.4
  
  MySQL / MariaDB
  
  Serveur local type WAMP, MAMP, XAMPP
  
  Navigateur Web (Chrome, Firefox, etc.)


📂 Installation du projet
  1. Cloner le dépôt
    > git clone https://github.com/ton-utilisateur/Five-Arena.git
    > cd 5arena-mvc

  2. Placer le projet dans le serveur local
    Exemple : C:/wamp64/www/5arena-mvc pour WAMP.
  
  3. Importer la base de données
    Ouvrir phpMyAdmin
     Créer une nouvelle base de données nommée fivearena
     Importer le fichier fivearena.sql
  
  4. Configurer la connexion à la base de données
    Modifier le fichier models/dbModels.php si nécessaire :
  
      $host = 'localhost';    
      $host = 'localhost:8080';    # Sur mac 🍎
      $dbname = 'fivearena';
      $username = 'root';
      $password = '';
      $password = 'root';          # Sur mac 🍎


🚀 Lancer le projet
  Démarrer le serveur local  
  Ouvrir dans le navigateur : http://localhost/votreChemin/5arena-mvc


🔐 Accès administrateur
  Identifiants admin :
    Email : adress@dom.com
    Mot de passe : 123

  Identifiants user :
    Email : adress@user.com
    Mot de passe : 123


📁 Structure du projet

  fivearena/
  ├── controllers/         → Logique des actions
  ├── models/              → Requêtes SQL & logique métier
  ├── views/               → Vues
  ├── public/
  │   ├── css/
  │   ├── js/
  │   ├── images/
  ├── index.php            → Point d’entrée principal
  └── fivearena.sql        → Base de données


✅ Fonctionnalités
  Authentification / Inscription
  
  Dashboard administrateur
  
  Ajout / modification / suppression de terrains
  
  Réservation de créneaux horaires
  
  Design responsive de base


📦 Technologies utilisées
  PHP (serveur)
  
  MySQL (base de données)
  
  HTML / CSS / JavaScript (front-end)
  
  Architecture MVC
