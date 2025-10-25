# StepUp

StepUp est une application mobile pour suivre ses habitudes quotidiennes.

## Technologies
- React Native
- Expo
- React Navigation

## Installation
1. Cloner le projet :  
   ```bash
   git clone https://github.com/ton-utilisateur/stepup.git
   cd stepup
   ```

2. Installer les dépendances :
  ```bash
  npm install
  ```

3. Lancer l’application :
   ```bash
   npm start
   ```
4.Scanner le QR code avec l’application Expo Go sur votre téléphone.

## Structure du projet
- App.js → point d’entrée de l’application
- components/ → composants réutilisables (Loading, Onboarding…)
- screens/ → écrans principaux (Splash, Login, Home…)
```
StepUp/
│
├── App.js                # Point d’entrée de l’application
├── package.json
├── assets/               # Images, icônes, logos
├── components/           # Composants réutilisables
│   ├── LoadingScreen.js
│   └── OnboardingStep.js
├── screens/              # Écrans principaux
│   ├── SplashScreen.js
│   ├── LoginScreen.js
│   ├── OnboardingScreen.js
│   └── HomeScreen.js
└── navigation/
    └── AppNavigator.js   # Gestion des routes et navigation
```

## Flux de l’application

Splash / Loading
Écran de lancement avec animation pendant le chargement initial.

Login / Inscription
Écran pour que l’utilisateur se connecte ou crée un compte.

Onboarding
Carrousel pour présenter les fonctionnalités principales aux nouveaux utilisateurs.
→ Sauvegarde dans le stockage local pour ne pas répéter l’onboarding.

Home
Écran principal pour visualiser et gérer ses habitudes.

## Fonctionnalités prévues
- Gestion des habitudes (création, modification, suppression)
- Choix d’habitudes prédéfinies par catégorie
- Suivi quotidien et rappels
- Notifications push (à implémenter)
- Onboarding interactif pour guider l’utilisateur

## Notes pour les contributeurs
Ce projet est développé avec React Native + Expo pour un démarrage rapide.
Chaque écran est séparé en composant pour faciliter la maintenance.
La navigation utilise React Navigation, et les données locales peuvent être gérées via AsyncStorage.
