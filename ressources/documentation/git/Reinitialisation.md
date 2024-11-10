# Réinitialisation

## A - Réinitialisation et restauration

- `git reset --hard <commit>` : Réinitialise l'historique et l'espace de travail à un commit spécifique (irréversible).
- Forcer la réinitialisation de la branche locale à l'état du dépôt distant :

  ```bash
  git fetch origin
  git reset --hard origin/nom_branche
  ```

- `git reset --hard <branche>` : Réinitialise la branche locale à l'état d'une autre branche (locale ou distante).
- `git restore --source <commit> -- <fichier>` : Restaure un fichier à partir d'un commit donné.
- **`git revert HEAD~N..HEAD`** : Annule les *N* derniers commits en conservant l'historique.

## B - Rebase et modification de l'historique

**Pas recommandé sur des branches partagées.**

- `git rebase HEAD~N` : Rebaser les N derniers commits.
- `git rebase -i <branche>` : Lancer un rebase interactif pour modifier l'historique des commits.
- `git commit --amend` : Modifier le dernier commit.
