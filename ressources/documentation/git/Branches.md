# Branches

Permet de créer des nouvelles fonctionnalités

## A - Fonctionnement

- branche principale : main / master
- Lorsqu'une branche est créée, tous les fichiers sont copiés dans celle-ci.
- Les modifications apportées sur la branche n'influent pas sur la branche d'origine.
- https://git-scm.com/book/fr/v2/Les-branches-avec-Git-Branches-et-fusions%C2%A0%3A-les-bases

## B - Commandes de base

- obtenir la branche actuelle : `git branch`

  "*" signifie qu'il s'agit de la branche de travail actuelle

- basculer entre les branches : `git checkout <nom-branche>` / `git switch <nom-branche>`
- arborescence du dépot : `git log --graph --oneline --all --decorate --topo-order`

## C - Créer une branche

1. créer : `git checkout -b <nom-branche>` / `git branch <nom-branche>`
2. afficher branches : `git branch`
3. mettre à jour : `git push --set-upstream origin <nom-branche>`

## D - Fusionner deux branches

### a) Fusionner (merge)

Ajoute un seul commit pour tout l'ajout

1. se déplacer dans la branche principale : `git checkout <branche-principale>`
2. fusionner : `git merge <branche-secondaire>`
3. **(optionnel)** supprimer : `git branch -d <branche-secondaire>`

### b) Rebaser (rebase)

Ajoute tous les commits de la branche

1. se déplacer dans la branche secondaire : `git checkout <branche-secondaire>`
2. rebaser (ajouter les commits) : `git rebase <branche-principale>`
3. se déplacer dans la branche principale : `git checkout <branche-principale>`
4. fusionner : `git merge <branche-secondaire>`
5. **(optionnel)** supprimer : `git branch -d <branche-secondaire>`

## E - Supprimer une branche

https://fr.w3docs.com/snippets/git/comment-supprimer-des-branches-locales-et-distantes-dans-git.html

### a) Localement

- `git branch -d <branche>`

### b) Distance

- `git push origin --delete <branche>`
