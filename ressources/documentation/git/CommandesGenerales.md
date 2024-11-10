# Commandes générales

## A - Mettre à jour distant vers local

- **`git pull`** : Mettre à jour distant vers local :
- **`git push`** : Mettre à jour local vers distant (sans conflits)
- `git fetch` : Met à jour les références locales du dépôt distant.

## B - Informations

- **`git status`** : Afficher l'état actuel des modifications et des fichiers suivis.
- **`git log`** : Lister l'historique des commits récents.
- `git log --oneline` : Lister l'historique des commits récents.

## C - Actions sur les fichiers

- **`git add <fichier>`** : Ajouter un fichier spécifique à l'index.
- **`git rm <fichier>`** : Supprimer un fichier du projet et de l'index.
- **`git restore <fichier>`** : Restaurer un fichier à son état d'origine.

## D - Commit

- **`git commit -m "..."`** : Créer un commit avec un message spécifique après un ajout.
- **`git commit --amend -m "Nouveau message"`** : Réécrire le dernier commit (utile pour modifier le message ou ajouter des fichiers).
- **`git reset HEAD^`** : Réinitialiser le dernier commit

## E - Fusionner projet local et projet distant (de manière sécurisée)

1. `git add .`
2. `git commit -m "..."`
3. `git pull`
4. Resoudre les conflits potentiels
5. `git add .`
6. `git commit -m "résolution des conflits"`
7. `git push`

## F - Mettre en pause et reprendre des modifications (sans commit)

- **`git stash`** : Mettre en pause les modifications actuelles et réinitialiser l'espace de travail.
- **`git stash list`** : Afficher la liste des stash.
- **`git stash apply`** : Réappliquer le dernier stash.
- `git stash apply stash@{N}` : Réappliquer un stash spécifique.
- `git stash branch <branche>` : créer une nouvelle branche à partir d'un stash
- **`git stash pop`** : Réappliquer le dernier stash et le supprimer de la liste.
- `git stash clear` : Supprimer tous les stash.

## A regarder

- git bisect
