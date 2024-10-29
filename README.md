# Projet d'Architecture Logicielle

Bienvenue dans le projet d'Architecture Logicielle  sur le sujet Groupes ! 
Ce dépôt contient le code source et les instructions pour collaborer efficacement. Veuillez suivre les règles de Git ci-dessous pour assurer une bonne gestion des versions et une collaboration harmonieuse.

## Prérequis

- **Java JDK** (version 8 ou plus) : [Télécharger ici](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
- **Un IDE** comme [IntelliJ IDEA](https://www.jetbrains.com/idea/download/) ou [Eclipse](https://www.eclipse.org/downloads/)
## Installation du Projet en Local

**Cloner le dépôt** :
   ```bash
   git clone https://github.com/awudza/archi_logicielle.git
   cd archi_logicielle
   ```
 
# Guide de Collaboration

Bienvenue dans notre projet Java Swing ! Afin d'assurer une organisation efficace, nous avons une **branche `develop`** qui sert de base pour toutes les nouvelles fonctionnalités et modifications. 

Chaque collaborateur doit **créer sa propre branche personnelle depuis `develop`** et y travailler exclusivement. Voici les règles pour une bonne gestion du dépôt.

## Règles de Base pour la Collaboration

### 1. Utilisation de la Branche `develop`

   - **Ne pas travailler directement dans `main` ni `develop`** : La branche `main` est réservée aux versions stables et prêtes pour la production. La branche `develop` sert de base pour toutes les nouvelles fonctionnalités, corrections et améliorations.
   - **Créer une branche personnelle depuis `develop`** : Dès que vous commencez une nouvelle tâche, créez une branche qui porte votre nom et le nom de la fonctionnalité ou tâche.
   
     - Exemple de nom de branche : `julie-authentification` ou `pierre-interface`.

     - Créez votre branche personnelle depuis `develop` :
       ```bash
       git checkout develop
       git pull origin develop
       git checkout -b votre-nom/nom-tache
       ```

### 2. Travailler Uniquement dans Votre Branche

   - **Restez dans votre branche personnelle** : Ne faites pas de modifications directement dans `develop`. Effectuez toutes vos modifications, tests et commits dans votre propre branche.
   - **Faire des commits fréquents** : Commitez régulièrement vos changements avec des messages descriptifs pour garder un historique clair de votre travail.

### 3. Synchroniser Votre Branche avec `develop`

   - **Mettre à jour `develop`** : Avant chaque session de travail, assurez-vous que `develop` est à jour :
     ```bash
     git checkout develop
     git pull origin develop
     ```
   - **Fusionner `develop` dans votre branche** : Ensuite, fusionnez les dernières modifications de `develop` dans votre branche personnelle pour éviter les conflits plus tard.
     ```bash
     git checkout votre-nom/nom-tache
     git merge develop
     ```

   - **Résoudre les conflits** : Si des conflits apparaissent pendant la fusion, résolvez-les dans votre branche personnelle. Testez ensuite votre code pour vérifier que tout fonctionne correctement.

### 4. Créer une Pull Request pour Fusionner dans `develop`

   - **Pull Request (PR)** : Une fois votre travail terminé, créez une Pull Request (PR) vers `develop` depuis votre branche personnelle.
   - **Supprimer la branche** : Après que la PR est fusionnée, supprimez votre branche personnelle pour garder le dépôt propre.

---

## Exemples de Commandes Git

- **Créer une branche personnelle depuis `develop`** :
  ```bash
  git checkout develop
  git pull origin develop
  git checkout -b votre-nom
  git add .
  git commit -m "message décrivant votre dépôt"
  git push origin branch
