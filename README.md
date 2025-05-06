# 📘 FiveArena – Documentation d'installation et d'utilisation

## 🧾 Présentation

**FiveArena** (5arena-mvc) est une application web développée en PHP avec une architecture MVC.  
Elle permet de gérer la réservation de terrains de sport (ajout, édition, suppression), la gestion des utilisateurs et des réservations via un back-office.

---

## 🛠️ Prérequis

- PHP ≥ 7.4  
- MySQL / MariaDB  
- Serveur local type **WAMP**, **MAMP**, **XAMPP**  
- Navigateur Web (Chrome, Firefox, etc.)

---

## 📂 Installation du projet

1. **Cloner le dépôt**  
   ```
   
   git clone https://github.com/ton-utilisateur/Five-Arena.git
   cd 5arena-mvc

   ```

2. **Placer le projet dans le serveur local**
  Exemple :
  
  ```
  
  C:/wamp64/www/5arena-mvc  (pour WAMP)

  ```
  
3. **Importer la base de données**
  
  - Ouvrir phpMyAdmin
  
  - Créer une base de données nommée fivearena
  
  - Importer le fichier fivearena.sql
  
  - Configurer la connexion à la base de données
  
  - Modifier models/dbModels.php si nécessaire :

    ```
  
    // Sur Windows / Linux
    private $host     = 'localhost';
    private $dbname   = 'fivearena';
    private $username = 'root';
    private $password = '';
    
    // Sur macOS (MAMP)
    private $host     = 'localhost:8080';
    private $dbname   = 'fivearena';
    private $username = 'root';
    private $password = 'root';

    ```

## 🚀 Lancer le projet
  1. **Démarrer votre serveur local**

  2. **Accéder à l’URL dans votre navigateur :**

     ```
     
     http://localhost/5arena-mvc/
     
     ```

## 🔐 Accès
  **Admin**
    - Email : adress@dom.com
    - Mot de passe : 123
  
  **Utilisateur**
  - Email : adress@user.com
  - Mot de passe : 123

## 📁 Structure du projet

  ```
  
  5arena-mvc/
  ├── controllers/        → Logique des actions
  ├── models/             → Requêtes SQL & logique métier
  ├── views/              → Vues (front & back-office)
  ├── public/
  │   ├── css/            → Styles
  │   ├── js/             → Scripts
  │   └── images/         → Assets images
  ├── index.php           → Routeur principal
  └── fivearena.sql       → Fichier de base de données
  
  ```

## ✅ Fonctionnalités
  - Authentification / Inscription
  - Dashboard administrateur
  - Ajout / modification / suppression de terrains
  - Réservation de créneaux horaires
  - Design responsive de base

## 📦 Technologies utilisées
  - PHP (serveur)
  - MySQL (base de données)
  - HTML / CSS / JavaScript (front-end)
  - Architecture MVC
