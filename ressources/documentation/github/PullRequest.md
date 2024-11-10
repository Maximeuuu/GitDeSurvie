# Utilisation des pull request

## 1. Copier un référenciel (fork)

1. accèder au référenciel github (lien)
2. créer un fork : `fork` > `create new fork` > `create fork`
3. copier le fork localement : `git clone <url>`

## 2. Création branche thématique

*Depuis le répertoire.*

1. créer une branche : `git checkout -b <branche>`
2. vérifier : `git branch`
3. synchroniser local -> distant : `git push origin <branche>`

## 3. Modifications sur la branche

1. faire des modifications
2. synchroniser localement (git status, git add, git commit)
3. synchroniser en distant (git push)

## 4. Proposer des modifications à un utilisateur (pull request)

1. Après avoir poussé la branche, GitHub propose de créer une pull request
2. Initier : Cliquer sur `compare & pull request`
3. Compléter la pull request
    - base : `main:<destinataire>`
    - compare : `<ma-branche>`
    - ajouter des commentaires
4. Cliquer sur `create pull request`

## 5. Accepter une pull request

1. Aller dans `github` > `pull resquest`
    - Analyer la demander : *conversation*, *commits*, *files changed*
    - Accepter si tout est OK : `merge pull request`
