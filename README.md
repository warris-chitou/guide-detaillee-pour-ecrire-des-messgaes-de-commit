# Guide des Messages de Commit

Les messages de commit doivent être clairs, concis, et suivre une structure qui permet de comprendre rapidement ce qui a été changé et pourquoi. Voici un guide étape par étape pour rédiger des messages de commit efficaces et suivre les bonnes pratiques.

## 1. Structure générale d’un message de commit

### Format classique :
```
<type>: <résumé court de la modification>

<description détaillée (facultative)>
```

#### Exemples de types courants :
- **feat:** nouvelle fonctionnalité
- **fix:** correction de bug
- **chore:** tâches administratives ou de maintenance
- **docs:** modifications dans la documentation
- **refactor:** refactorisation sans changement de fonctionnalité
- **style:** modifications liées au style de code
- **test:** ajout ou modification de tests

## 2. Écrire un message de commit clair et concis

### En-tête :
- Soyez direct et précis. Résumez l’action principale en **moins de 50 caractères**.
- Utilisez un verbe à l’infinitif : **"ajouter"**, **"corriger"**, **"modifier"**.
- **Exemples :**
  - `fix: corriger l'affichage des articles sur mobile`
  - `feat: ajouter la gestion des filtres dans la recherche`

### Description détaillée (facultative) :
- Ajoutez des détails si nécessaire, en **72 caractères maximum par ligne**.
- Expliquez *pourquoi* et *comment* la modification a été faite.
- **Exemple :**
```
fix: corriger l'affichage des articles sur mobile

- Résolution du problème d'affichage des images sur les écrans étroits.
- Correction des marges et de l'espacement pour la version mobile.
- Le layout est maintenant responsive grâce à Flexbox.
```

## 3. Utilisation des préfixes (`type:`)
- **fix:** pour les corrections de bugs.
- **Exemple :**
```
fix: corriger le bug de la responsivité sur la page d'accueil
```

## 4. Autres bonnes pratiques pour rédiger des messages de commit

### a. Soyez spécifique mais concis
- **Mauvais exemple** : `Correction d'un bug`
- **Bon exemple** : `fix: corriger le bug de décalage des images sur mobile`

### b. Utilisez l’impératif
- **Correct** : `fix: corriger l’affichage des images sur la page d’accueil`
- **Incorrect** : `fix: a corrigé l’affichage des images sur la page d’accueil`

### c. Contexte du commit
- Ajoutez un identifiant de tâche ou de bug pour la traçabilité.
- **Exemple** : `fix: corriger l'affichage des articles sur mobile (JIRA-123)`

### d. Séparer les modifications
- Si un commit contient plusieurs changements, séparez-les en plusieurs commits distincts.

## 5. Exemples de messages de commit en français

### Pour un bug :
```
fix: corriger le bug de l'affichage des articles sur mobile
```
#### Description détaillée :
```
fix: corriger le bug de l'affichage des articles sur mobile

- Le layout des articles n'était pas correctement affiché sur les petits écrans.
- Ajout de Flexbox pour rendre les articles responsives.
```

### Pour une fonctionnalité :
```
feat: ajouter un système de filtrage des articles
```
#### Description détaillée :
```
feat: ajouter un système de filtrage des articles

- Mise en place des filtres par catégorie et par date.
- Ajout d'un sélecteur de date avec un calendrier.
```

### Pour une refactorisation :
```
refactor: réorganiser les fichiers CSS pour améliorer la maintenabilité
```
#### Description détaillée :
```
refactor: réorganiser les fichiers CSS pour améliorer la maintenabilité

- Séparation des styles en plusieurs fichiers plus petits.
- Utilisation de variables CSS pour une meilleure cohérence.
```

## 6. Outils utiles pour améliorer les messages de commit
- **Commitlint** : vérifie que vos messages respectent un format prédéfini.
- **Conventional Commits** : définit des règles sur les types de commits pour rendre l’historique plus lisible.

## En résumé :
- Utilisez des préfixes clairs (`feat:`, `fix:`, `chore:`, etc.).
- Rédigez des messages concis et informatifs, en utilisant l'impératif.
