# GDN - Gestion Des Notes (Student Grade Management System)

## 📋 Description

GDN (Gestion Des Notes) est une application desktop développée en C++ avec Qt pour la gestion des notes d'étudiants. Cette application permet aux enseignants et responsables pédagogiques de gérer efficacement les données académiques des étudiants.

## 🛠️ Technologies Utilisées

- **Language**: C++11
- **Framework**: Qt (Qt Widgets, Qt SQL)
- **Base de données**: SQLite
- **IDE**: Qt Creator
- **Système de build**: qmake

## 📁 Structure du Projet

```
C-mini-projet/
├── README.md
└── P C++/
    ├── main.cpp              # Point d'entrée de l'application
    ├── Widget.cpp/h          # Classe principale et gestion de la base de données
    ├── menu1.cpp/h           # Interface du menu principal
    ├── menu2.cpp/h           # Interface du menu secondaire
    ├── *.ui                  # Fichiers d'interface utilisateur Qt
    ├── GDN.pro               # Fichier de configuration Qt
    ├── *.png                 # Ressources graphiques
    └── Database/
        └── Database.db       # Base de données SQLite
```

## ⚙️ Fonctionnalités

Le système de gestion des notes offre les fonctionnalités suivantes :

- **➕ Ajouter** : Insertion de nouvelles données d'étudiants et de notes
- **📝 Modifier** : Modification des informations existantes
- **🗑️ Supprimer** : Suppression de données d'étudiants ou de notes
- **👁️ Afficher** : Visualisation des données et des rapports
- **🔐 Authentification** : Système de connexion sécurisé

## 🚀 Installation et Compilation

### Prérequis

- Qt 5.x ou supérieur
- Qt Creator (recommandé)
- Compilateur C++ compatible C++11
- SQLite (inclus avec Qt)

### Étapes d'installation

1. **Cloner le repository**

   ```bash
   git clone https://github.com/el-houfi-achraf/C-mini-projet.git
   cd C-mini-projet
   ```

2. **Ouvrir le projet**

   - Ouvrir Qt Creator
   - Fichier → Ouvrir un fichier ou projet
   - Sélectionner `P C++/GDN.pro`

3. **Compiler et exécuter**
   - Appuyer sur Ctrl+R ou cliquer sur le bouton "Exécuter"
   - Ou utiliser la ligne de commande :
     ```bash
     cd "P C++"
     qmake
     make
     ./GDN
     ```

## 📊 Base de Données

L'application utilise une base de données SQLite stockée dans `Database/Database.db`. La structure inclut :

- **Données des étudiants** : Informations personnelles et académiques
- **Cours** : Matières et modules d'enseignement
- **Notes** : Évaluations et résultats
- **Enseignants** : Informations du personnel pédagogique

## 🖼️ Interface Utilisateur

L'application dispose d'une interface graphique intuitive avec :

- **Écran de connexion** : Authentification des utilisateurs
- **Menu principal** : Navigation entre les différentes fonctionnalités
- **Formulaires de saisie** : Interfaces pour ajouter/modifier les données
- **Tableaux d'affichage** : Visualisation des données sous forme tabulaire

## 🔧 Configuration

La configuration de la base de données se trouve dans `Widget.cpp` :

```cpp
mydb.setDatabaseName("C:/Users/ACHRAF/Downloads/P C++/Database/Database.db");
```

⚠️ **Important** : Modifier le chemin de la base de données selon votre environnement.

## 📝 Utilisation

1. **Démarrer l'application**
2. **Se connecter** avec vos identifiants
3. **Naviguer** dans le menu pour accéder aux fonctionnalités
4. **Gérer les données** : ajouter, modifier, supprimer ou afficher les informations

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. Fork le projet
2. Créer une branche pour votre fonctionnalité (`git checkout -b feature/AmazingFeature`)
3. Commit vos changements (`git commit -m 'Add some AmazingFeature'`)
4. Push vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrir une Pull Request

## 👨‍💻 Auteur

**Achraf El Houfi** - [el-houfi-achraf](https://github.com/el-houfi-achraf)

## 📞 Support

Pour toute question ou problème, n'hésitez pas à ouvrir une issue sur le repository GitHub.

---

_La gestion des notes des étudiants repose sur une structure solide, englobant les données des étudiants, des cours, des notes et des enseignants. La logique de l'application, du suivi des notes à la validation et la notification, assure un processus transparent. Les interactions entre les données permettent aux enseignants de saisir les notes, aux responsables pédagogiques d'analyser la performance, et aux étudiants de suivre leur progression. Grâce à l'utilisation d'une base de données, la gestion des données académiques est organisée, sécurisée et accessible, favorisant l'efficacité du processus global._
