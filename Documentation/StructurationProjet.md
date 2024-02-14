Branches
===

Permet de créer des nouvelles fonctionnalités

https://git-scm.com/book/fr/v2/Les-branches-avec-Git-Branches-et-fusions%C2%A0%3A-les-bases

## A - Fonctionnement
- branche principale : main / master
- Lorsqu'une branche est créée, tous les fichiers sont copiés dans celle-ci.
- Les modifications apportées sur la branche n'influent pas sur la branche d'origine.

## B - Commandes de base
- obtenir la branche actuelle : `git branch`
   - "*" signifie qu'il s'agit de la branche de travail actuelle
- basculer entre les branches : `git checkout <nom-branche>`
- arborescence du dépot       : `git log --graph --oneline --all --decorate --topo-order`

## C - Créer une branche
1. créer             : `git checkout -b <nom-branche>`
2. afficher branches : `git branch`
3. mettre à jour     : `git push --set-upstream origin <nom-branche>`

## D - Fusionner deux branches
1. se déplacer dans la branche principale : `git checkout <nom-branche-principale>`
2. fusionner : `git merge <nom-branche>`
3. supprimer : `git branch -d <nom-branche>`
