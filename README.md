# ProDev Mobile App - React Native avec Expo Router

Ce projet démontre l'implémentation d'une application mobile React Native utilisant Expo Router pour la navigation.

## Projets Créés

### prodev-mobile-app-0x04 - Stack Navigation
- Navigation en pile (Stack Navigation)
- Écrans : Index, Join, Sign In
- Utilisation de fichiers de style séparés
- Images d'assets personnalisées

### prodev-mobile-app-0x05 - Tab Navigation (En cours)
- Navigation par onglets (Tab Navigation)
- Écrans : Home, Search, Saved, Inbox, Profile
- Composants réutilisables pour les propriétés
- Interface utilisateur avec cartes de propriétés

## Structure du Projet

```
app/
├── _layout.tsx          # Configuration de navigation principale
├── index.tsx            # Écran d'accueil
├── join.tsx             # Écran d'inscription
├── signin.tsx           # Écran de connexion
└── (home)/              # Groupe d'onglets
    ├── _layout.tsx      # Configuration des onglets
    ├── index.tsx        # Accueil avec listings
    ├── search.tsx       # Recherche
    ├── saved.tsx        # Favoris
    ├── inbox.tsx        # Messages
    └── profile.tsx      # Profil

components/
├── common/
│   └── PropertyListingCard.tsx
└── PropertyListing.tsx

styles/
├── _mainstyle.ts        # Styles principaux
├── _joinstyle.ts        # Styles formulaires
├── _homestyle.ts        # Styles accueil
└── _propertyCardStyle.ts # Styles cartes

constants/
├── index.ts             # Constantes d'assets
└── data.ts              # Données de test

interfaces/
└── index.ts             # Types TypeScript
```

## Fonctionnalités

### Navigation Stack (0x04)
- ✅ Écran d'accueil avec image de fond
- ✅ Navigation vers inscription/connexion
- ✅ Formulaires avec validation visuelle
- ✅ Boutons avec icônes sociales
- ✅ Interface responsive

### Navigation Tabs (0x05)
- ✅ Configuration des onglets avec icônes
- ✅ Écran d'accueil avec recherche
- ✅ Filtres horizontaux
- ✅ Cartes de propriétés avec images
- ✅ Composants réutilisables
- 🚧 Données simulées
- 🚧 Images placeholder nécessaires

## Installation et Utilisation

```bash
# Installer les dépendances
cd prodev-mobile-app-0x04  # ou prodev-mobile-app-0x05
npm install

# Démarrer l'application
npx expo start

# Scanner le QR code avec Expo Go (mobile)
# Ou ouvrir dans un simulateur
```

## Assets Requis

Les images suivantes sont nécessaires dans `assets/images/` :

**Pour 0x04 :**
- hero-icon.png (image de fond)
- Logo.png (logo principal)
- logo-green.png (logo vert)
- google.png (logo Google)
- facebook.png (logo Facebook)

**Pour 0x05 (en plus) :**
- sample-image.png (image de propriété)
- mansion.png (icône filtre)
- user-image.png (avatar utilisateur)

## Technologies Utilisées

- React Native
- Expo Router v5
- TypeScript
- Expo Vector Icons
- StyleSheet API

## Prochaines Étapes

1. **Tâche 2 :** Intégration NativeWind (TailwindCSS)
2. **Tâche 3 :** Défi d'implémentation UI
3. Ajout d'images d'assets réelles
4. Implémentation de l'authentification
5. Connexion à une API de données

## Problèmes Connus

- Les imports avec `@/` peuvent nécessiter une configuration TypeScript supplémentaire
- Certaines images placeholder manquent
- La navigation vers les onglets groupés nécessite un debugging supplémentaire

## Liens Utiles

- [Documentation Expo Router](https://docs.expo.dev/router/introduction/)
- [Expo Vector Icons](https://docs.expo.dev/guides/icons/)
- [React Navigation](https://reactnavigation.org/)
