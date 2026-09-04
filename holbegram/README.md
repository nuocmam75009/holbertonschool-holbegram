# Holbegram

Holbegram est une application mobile inspirée d'Instagram, développée en **Flutter** avec **Firebase** comme backend (authentification, base de données et stockage). Ce projet a été réalisé dans le cadre du cursus Holberton School.

## Fonctionnalités

- **Authentification** : inscription et connexion des utilisateurs (Firebase Auth)
- **Fil d'actualité (Feed)** : affichage des publications
- **Publication d'images** : ajout de photos depuis la galerie
- **Recherche** : recherche d'utilisateurs ou de contenus
- **Favoris** : sauvegarde des publications préférées
- **Profil** : consultation et gestion du profil utilisateur

## Stack technique

- [Flutter](https://flutter.dev/) / Dart
- [Firebase](https://firebase.google.com/) (Auth, Cloud Firestore, Storage)
- `provider` pour la gestion d'état
- `image_picker` pour la sélection d'images
- `bottom_navy_bar` pour la navigation

## Structure du projet

```
lib/
├── main.dart                  # Point d'entrée de l'application
├── methods/                   # Méthodes d'authentification
├── models/                    # Modèles de données (User, Posts)
├── providers/                 # Gestion d'état (UserProvider)
├── screens/
│   ├── login_screen.dart
│   ├── signup_screen.dart
│   ├── upload_image_screen.dart
│   ├── home.dart
│   ├── Pages/                 # Feed, Search, AddImage, Favorite, Profile
│   └── auth/methods/          # Stockage utilisateurs et publications
├── utils/
└── widgets/                   # Composants réutilisables (text_field, bottom_nav)
```

## Installation

### Prérequis

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (>= 3.3.3)
- Un projet [Firebase](https://console.firebase.google.com/) configuré

### Étapes

1. Cloner le dépôt
   ```bash
   git clone https://github.com/nuocmam75009/holbertonschool-holbegram.git
   cd holbertonschool-holbegram/holbegram
   ```

2. Installer les dépendances
   ```bash
   flutter pub get
   ```

3. Configurer Firebase
   - Ajouter votre fichier `google-services.json` dans `android/app/`
   - Renseigner vos identifiants Firebase dans `lib/firebase_options.dart` (ou via `flutterfire configure`)

4. Lancer l'application
   ```bash
   flutter run
   ```

## Auteurs

Projet réalisé dans le cadre de la formation Holberton School.
