**Nom :** Maxime Lemoine

**Groupe :** B

**Année :** 2023

**IUT Le Havre - Cours GIT**

---

# Compte-rendu TP2 - GitHub
[tp2](https://abderzah.github.io/Introduction-GIT/tp2/)

Dans ce TP on apprend à travailler avec github.
GitHub permet un dépot distant

## Configuration
1. créer une clé publique ssh : `ssh-keygen`
2. récupérer une clé          : `cat ~/.ssh/id_rsa.pub`
3. ajout dans github          : `settings` > `SSH and GPG keys` > `Nouvelle clé SSH`

## Pousser un dépot
### sur github
1. créer un répertoire : `github.io` > `new repository`
- accéder via le site  : `https://github.com/<utilisateur>/<dossier>.git`
- connexion via ssh    : `git@github.com:<utilisateur>/<dossier>.git`

### dans le repertoire local
dans `<repertoire>/<dossier>`

2. verifier si le repertoire existe déjà     : `git remote -v`
3. lier le dépot local et répertoire distant : `git remote add origin <utilisateur>/<dossier>.git`
4. nom de la branche (main/master)           : `git branch`
5. créer un lien permanant et maj dépot      : `git push -u origin master`

## Sychroniser local et distant
### commandes générales
- ajouter un dépot distant        : `git remote`
- mettre à jour le dépot distant  : `git push`
- mettre à jour le dépot local    : `git pull`

- voir les modifications récentes : `git log`

### mettre à jour local -> distant
1. `git status`
2. `git add <element>`
3. `git commit -m "<Commentaire>"`
4. `git push`

### mettre à jour distant -> local
1. `git pull origin main`

### Cloner un dépot disant -> local
1. dans le répertoire parent : `git clone git@github.com:<utilisateur>/<repertoire>.git`


