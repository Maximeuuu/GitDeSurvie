Configuration de l'outil GIT
===

## A - Configuration utilisateur

- liste des configuration : `git config --list`
- ajouter un auteur : `git config --global user.name "Maxime L"`
- ajouter un email  : `git config --global user.email "maxime.lemoine1@etu.univ-lehavre.fr"`


## B - Configuration SSH

1. créer une clé publique ssh : `ssh-keygen`
2. récupérer une clé          : `cat ~/.ssh/id_rsa.pub`
3. ajout dans github          : `settings` > `SSH and GPG keys` > `Nouvelle clé SSH`
