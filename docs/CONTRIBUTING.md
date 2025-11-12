# 🤝 Guide de Contribution

Bienvenue à tous les collaborateurs de l'équipe sur ce mini-projet !

Pour assurer un `git log` propre et une collaboration fluide, veuillez suivre rigoureusement les conventions ci-dessous.

## 1. Organisation des Branches

Nous utilisons une approche de "Feature Branching" simplifiée.

* **`main`** : Branche stable, contient le projet validé final.
* **`dev`** : Branche de développement principale, elle agrège les branches individuelles. Toutes les Pull Requests sont d'abord fusionnées ici.
* **Branches Personnelles (`feature/nom-utilisateur`)** :
    * **Chaque membre DOIT créer et travailler exclusivement** sur sa propre branche individuelle (ex: `feature/paul`) pour toutes ses modifications initiales

## 2. Conventions de Commits

Nous adoptons une structure de messages de commits standardisée pour maintenir un historique clair

Le format est : `[type]: description détaillée`

| Type | Description |
| :--- | :--- |
| **`feat`** | Ajout d'une nouvelle fonctionnalité (ex: ajout d'un fichier de contenu)
| **`fix`** | Correction d'un bug  |
| **`docs`** | Changement de la documentation (ex: README, CONTRIBUTING, etc.)
| **`style`** | Changements de formatage, pas de changement dans le code (espaces, virgules, etc.)
| **`refactor`**| Restructuration du code sans changement de fonctionnalité
| **`chore`** | Maintenance, changements n'impactant pas le code source (ex: mise à jour de .gitignore, ajout de licence)

**Exemples de messages de commit propres :**

* `feat: ajout de l'introduction personnelle dans index.txt`
* `docs: ajout de LICENCE.md avec la licence du projet`
* `fix: correction de la faute de frappe dans partie1.txt`

## 3. Historique Git Propre (`git log`)

**Avant d'ouvrir une Pull Request (PR) :**

1.  **Nettoyez vos commits :** Utilisez `git rebase -i` sur votre branche personnelle (`feature/nom-utilisateur`) pour *squasher* (fusionner) les commits intermédiaires, peu explicites ou superflus. L'objectif est d'avoir un commit unique et significatif par tâche
2.  **Le `git log` final doit être clair et significatif**

## 4. Gestion des Pull Requests (PR)

1.  Lorsque vos modifications sont terminées sur votre branche personnelle, ouvrez une PR pour fusionner vers la branche **`dev`**[.
2.  **Une validation est obligatoire :** Un autre membre de l'équipe doit commenter et **approuver** la PR avant sa fusion[
3.  **PR finale (`dev` vers `main`) :** Une PR finale unique sera créée pour fusionner `dev` dans `main`, en s'assurant que l'historique de `dev` est parfaitement propre avant cette étape
